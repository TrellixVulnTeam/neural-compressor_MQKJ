Validated Models
===
## Validated MLPerf Models
<table class="docutils">
<thead>
  <tr>
    <th>Model</th>
    <th>Framework</th>
    <th>Support</th>
    <th>Example</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="2">ResNet50 V1.5</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="../examples/tensorflow/image_recognition/tensorflow_models/quantization/ptq">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/image_recognition/torchvision_models/quantization/ptq/cpu/ipex">Link</a></td>
  </tr>
  <tr>
    <td>DLRM</td>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/recommendation/dlrm/quantization/ptq">Link</a></td>
  </tr>
  <tr>
    <td rowspan="2">BERT large</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="../examples/tensorflow/nlp/bert_large_squad/quantization/ptq">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/nlp/huggingface_models/question-answering/quantization/ptq_static/ipex">Link</a></td>
  </tr>
  <tr>
    <td rowspan="2">SSD ResNet34</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="../examples/tensorflow/object_detection/tensorflow_models/quantization/ptq">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/object_detection/ssd_resnet34/quantization">Link</a></td>
  </tr>
  <tr>
    <td>RNN-T</td>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/speech_recognition/rnnt/quantization">Link</a></td>    
  </tr>
  <tr>
    <td rowspan="2">3D-UNet</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="../examples/tensorflow/semantic_image_segmentation/3dunet-mlperf/quantization">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="../examples/pytorch/image_recognition/3d-unet/quantization">Link</a></td>
  </tr>
</tbody>
</table>

## Validated Quantization Examples

Performance results test on ​​09/24/2022 with Intel Xeon Platinum 8380 Scalable processor, using 1 socket, 4 cores/instance, 10 instances and batch size 1. 

Performance varies by use, configuration and other factors. See [platform configuration](./platform_configuration.md) for configuration details. For more complete information about performance and benchmark results, visit www.intel.com/benchmarks

### TensorFlow models with TensorFlow 2.10.0

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th rowspan="2">Example</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput(samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Accuracy Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td>EfficientNet</td>
    <td>pb</td>
    <td>76.74%</td>
    <td>76.76%</td>
    <td>-0.03%</td>
    <td>91.43</td>
    <td>69.41</td>
    <td>1.32x</td>
  </tr>
  <tr>
    <td>Faster R-CNN Inception ResNet V2</td>
    <td>pb</td>
    <td>37.65%</td>
    <td>38.33%</td>
    <td>-1.77%</td>
    <td>2.53</td>
    <td>1.62</td>
    <td>1.57x</td>
  </tr>
  <tr>
    <td>Faster R-CNN Inception ResNet V2 </td>
    <td>SavedModel</td>
    <td>37.77%</td>
    <td>38.33%</td>
    <td>-1.46%</td>
    <td>2.54</td>
    <td>1.61</td>
    <td>1.58x</td>
  </tr>
  <tr>
    <td>Faster R-CNN ResNet101</td>
    <td>pb</td>
    <td>30.34%</td>
    <td>30.39%</td>
    <td>-0.16%</td>
    <td>27.63</td>
    <td>13.12</td>
    <td>2.11x</td>
  </tr>
  <tr>
    <td>Faster R-CNN ResNet101</td>
    <td>SavedModel</td>
    <td>30.33%</td>
    <td>30.39%</td>
    <td>-0.20%</td>
    <td>27.71</td>
    <td>11.06</td>
    <td>2.51x</td>
  </tr>
  <tr>
    <td>Faster R-CNN ResNet50</td>
    <td>pb</td>
    <td>26.65%</td>
    <td>26.59%</td>
    <td>0.23%</td>
    <td>33.64</td>
    <td>16.33</td>
    <td>2.06x</td>
  </tr>
  <tr>
    <td>Inception ResNet V2</td>
    <td>pb</td>
    <td>80.34%</td>
    <td>80.40%</td>
    <td>-0.07%</td>
    <td>29.25</td>
    <td>23.43</td>
    <td>1.25x</td>
  </tr>
  <tr>
    <td>Inception V1</td>
    <td>pb</td>
    <td>70.44%</td>
    <td>69.74%</td>
    <td>1.00%</td>
    <td>163.14</td>
    <td>133.44</td>
    <td>1.22x</td>
  </tr>
  <tr>
    <td>Inception V2</td>
    <td>pb</td>
    <td>74.34%</td>
    <td>73.97%</td>
    <td>0.50%</td>
    <td>133.49</td>
    <td>111.5</td>
    <td>1.20x</td>
  </tr>
  <tr>
    <td>Inception V3</td>
    <td>pb</td>
    <td>76.71%</td>
    <td>76.75%</td>
    <td>-0.05%</td>
    <td>91.67</td>
    <td>64.02</td>
    <td>1.43x</td>
  </tr>
  <tr>
    <td>Inception V4</td>
    <td>pb</td>
    <td>80.18%</td>
    <td>80.27%</td>
    <td>-0.11%</td>
    <td>56.87</td>
    <td>37.09</td>
    <td>1.53x</td>
  </tr>
  <tr>
    <td>Mask R-CNN Inception V2</td>
    <td>pb</td>
    <td>28.50%</td>
    <td>28.73%</td>
    <td>-0.80%</td>
    <td>36.06</td>
    <td>27.15</td>
    <td>1.33x</td>
  </tr>
  <tr>
    <td>Mask R-CNN Inception V2 </td>
    <td>CKPT</td>
    <td>28.50%</td>
    <td>28.73%</td>
    <td>-0.80%</td>
    <td>36.1</td>
    <td>25.06</td>
    <td>1.44x</td>
  </tr>
  <tr>
    <td>MobileNet V1</td>
    <td>pb</td>
    <td>71.85%</td>
    <td>70.96%</td>
    <td>1.25%</td>
    <td>374.38</td>
    <td>226.03</td>
    <td>1.66x</td>
  </tr>
  <tr>
    <td>MobileNet V2</td>
    <td>pb</td>
    <td>71.85%</td>
    <td>70.96%</td>
    <td>1.25%</td>
    <td>374.38</td>
    <td>226.03</td>
    <td>1.66x</td>
  </tr>
  <tr>
    <td>ResNet101</td>
    <td>pb</td>
    <td>77.50%</td>
    <td>76.45%</td>
    <td>1.37%</td>
    <td>92.47</td>
    <td>65.56</td>
    <td>1.41x</td>
  </tr>
  <tr>
    <td>ResNet50 Fashion</td>
    <td>pb</td>
    <td>78.04%</td>
    <td>78.12%</td>
    <td>-0.10%</td>
    <td>359.18</td>
    <td>244.38</td>
    <td>1.47x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.0</td>
    <td>pb</td>
    <td>74.11%</td>
    <td>74.27%</td>
    <td>-0.22%</td>
    <td>172.66</td>
    <td>87.28</td>
    <td>1.98x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.5</td>
    <td>pb</td>
    <td>76.23%</td>
    <td>76.46%</td>
    <td>-0.30%</td>
    <td>153.37</td>
    <td>87.24</td>
    <td>1.76x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1</td>
    <td>pb</td>
    <td>23.12%</td>
    <td>23.13%</td>
    <td>-0.04%</td>
    <td>151.92</td>
    <td>112.24</td>
    <td>1.35x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1</td>
    <td>CKPT</td>
    <td>23.11%</td>
    <td>23.13%</td>
    <td>-0.09%</td>
    <td>153.18</td>
    <td>67.79</td>
    <td>2.26x</td>
  </tr>
  <tr>
    <td>SSD ResNet34</td>
    <td>pb</td>
    <td>21.71%</td>
    <td>22.09%</td>
    <td>-1.72%</td>
    <td>30.99</td>
    <td>8.65</td>
    <td>3.58x</td>
  </tr>
  <tr>
    <td>SSD ResNet50 V1</td>
    <td>pb</td>
    <td>37.76%</td>
    <td>38.00%</td>
    <td>-0.63%</td>
    <td>23.04</td>
    <td>14.75</td>
    <td>1.56x</td>
  </tr>
  <tr>
    <td>SSD ResNet50 V1</td>
    <td>CKPT</td>
    <td>37.82%</td>
    <td>38.00%</td>
    <td>-0.47%</td>
    <td>23</td>
    <td>11.94</td>
    <td>1.93x</td>
  </tr>
  <tr>
    <td>VGG16</td>
    <td>pb</td>
    <td>72.64%</td>
    <td>70.89%</td>
    <td>2.47%</td>
    <td>178.99</td>
    <td>83.67</td>
    <td>2.14x</td>
  </tr>
  <tr>
    <td>VGG19</td>
    <td>pb</td>
    <td>72.69%</td>
    <td>71.01%</td>
    <td>2.37%</td>
    <td>156.11</td>
    <td>71.5</td>
    <td>2.18x</td>
  </tr>
</tbody>
</table>

### PyTorch models with Torch 1.12.1+cpu in PTQ mode

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th rowspan="2">Example</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput (samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Acc Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td>ALBERT base MRPC</td>
    <td>EAGER</td>
    <td>88.85%</td>
    <td>88.50%</td>
    <td>0.40%</td>
    <td>26</td>
    <td>21.22</td>
    <td>1.23x</td>
  </tr>
  <tr>
    <td>Barthez MRPC</td>
    <td>EAGER</td>
    <td>83.92%</td>
    <td>83.81%</td>
    <td>0.14%</td>
    <td>128.66</td>
    <td>70.86</td>
    <td>1.82x</td>
  </tr>
  <tr>
    <td>BERT base MRPC</td>
    <td>FX</td>
    <td>89.90%</td>
    <td>90.69%</td>
    <td>-0.88%</td>
    <td>203.38</td>
    <td>101.29</td>
    <td>2.01x</td>
  </tr>
  <tr>
    <td>BERT base RTE</td>
    <td>FX</td>
    <td>69.31%</td>
    <td>69.68%</td>
    <td>-0.53%</td>
    <td>216.22</td>
    <td>102.72</td>
    <td>2.10x</td>
  </tr>
  <tr>
    <td>BERT base SST2</td>
    <td>FX</td>
    <td>91.06%</td>
    <td>91.86%</td>
    <td>-0.88%</td>
    <td>218.2</td>
    <td>101.86</td>
    <td>2.14x</td>
  </tr>
  <tr>
    <td>BERT base STSB</td>
    <td>FX</td>
    <td>64.12%</td>
    <td>62.57%</td>
    <td>2.48%</td>
    <td>73.65</td>
    <td>29.61</td>
    <td>2.49x</td>
  </tr>
  <tr>
    <td>BERT large COLA</td>
    <td>FX</td>
    <td>92.79</td>
    <td>93.16</td>
    <td>-0.39%</td>
    <td>36.54</td>
    <td>9.89</td>
    <td>3.70x</td>
  </tr>
  <tr>
    <td>BERT large MRPC</td>
    <td>FX</td>
    <td>89.50%</td>
    <td>90.38%</td>
    <td>-0.97%</td>
    <td>74.11</td>
    <td>29.69</td>
    <td>2.50x</td>
  </tr>
  <tr>
    <td>BERT large QNLI</td>
    <td>FX</td>
    <td>90.90%</td>
    <td>91.82%</td>
    <td>-1.00%</td>
    <td>72.45</td>
    <td>29.66</td>
    <td>2.44x</td>
  </tr>
  <tr>
    <td>BERT large RTE</td>
    <td>FX</td>
    <td>73.65%</td>
    <td>74.01%</td>
    <td>-0.49%</td>
    <td>41.53</td>
    <td>29.67</td>
    <td>1.40x</td>
  </tr>
  <tr>
    <td>BlendCNN</td>
    <td>EAGER</td>
    <td>68.40%</td>
    <td>68.40%</td>
    <td>0.00%</td>
    <td>3878.48</td>
    <td>3717.52</td>
    <td>1.04x</td>
  </tr>
  <tr>
    <td>CamemBERT base MRPC</td>
    <td>EAGER</td>
    <td>86.70%</td>
    <td>86.82%</td>
    <td>-0.14%</td>
    <td>188.97</td>
    <td>98.9</td>
    <td>1.91x</td>
  </tr>
  <tr>
    <td>Ctrl MRPC</td>
    <td>EAGER</td>
    <td>81.87%</td>
    <td>81.22%</td>
    <td>0.80%</td>
    <td>18.68</td>
    <td>7.25</td>
    <td>2.58x</td>
  </tr>
  <tr>
    <td>Deberta MRPC</td>
    <td>EAGER</td>
    <td>90.88%</td>
    <td>90.91%</td>
    <td>-0.04%</td>
    <td>124.43</td>
    <td>68.74</td>
    <td>1.81x</td>
  </tr>
  <tr>
    <td class="tg-zk71">DistilBERT base MRPC</td>
    <td>EAGER</td>
    <td>88.23%</td>
    <td>89.16%</td>
    <td>-1.05%</td>
    <td>347.47</td>
    <td>200.76</td>
    <td>1.73x</td>
  </tr>
  <tr>
    <td>DistilBERT base MRPC FX</td>
    <td>FX</td>
    <td>88.54%</td>
    <td>89.16%</td>
    <td>-0.69%</td>
    <td>382.74</td>
    <td>198.25</td>
    <td>1.93x</td>
  </tr>
  <tr>
    <td>FlauBERT MRPC</td>
    <td>EAGER</td>
    <td>79.87%</td>
    <td>80.19%</td>
    <td>-0.40%</td>
    <td>561.35</td>
    <td>370.2</td>
    <td>1.52x</td>
  </tr>
  <tr>
    <td>HuBERT</td>
    <td>FX</td>
    <td>97.69%</td>
    <td>97.84%</td>
    <td>-0.15%</td>
    <td>9.82</td>
    <td>7.2</td>
    <td>1.36x</td>
  </tr>
  <tr>
    <td class="tg-zk71">Inception V3</td>
    <td>EAGER</td>
    <td>69.43%</td>
    <td>69.52%</td>
    <td>-0.13%</td>
    <td>409.34</td>
    <td>181.95</td>
    <td>2.25x</td>
  </tr>
  <tr>
    <td>Longformer MRPC</td>
    <td>EAGER</td>
    <td>91.01%</td>
    <td>91.46%</td>
    <td>-0.49%</td>
    <td>18.73</td>
    <td>14.66</td>
    <td>1.28x</td>
  </tr>
  <tr>
    <td>mBart WNLI</td>
    <td>EAGER</td>
    <td>56.34%</td>
    <td>56.34%</td>
    <td>0.00%</td>
    <td>54.35</td>
    <td>25.14</td>
    <td>2.16x</td>
  </tr>
  <tr>
    <td class="tg-zk71">MobileNet V2</td>
    <td>EAGER</td>
    <td>70.54%</td>
    <td>71.84%</td>
    <td>-1.81%</td>
    <td>639.87</td>
    <td>490.05</td>
    <td>1.31x</td>
  </tr>
  <tr>
    <td class="tg-zk71">lvwerra/pegasus-samsum</td>
    <td>EAGER</td>
    <td>42.1</td>
    <td>42.67</td>
    <td>-1.35%</td>
    <td>3.41</td>
    <td>1.07</td>
    <td>3.19x</td>
  </tr>
  <tr>
    <td class="tg-zk71">PeleeNet</td>
    <td>EAGER</td>
    <td>71.64%</td>
    <td>72.10%</td>
    <td>-0.64%</td>
    <td>419.42</td>
    <td>316.98</td>
    <td>1.32x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNet18 </td>
    <td>EAGER</td>
    <td>69.57%</td>
    <td>69.76%</td>
    <td>-0.27%</td>
    <td>686.03</td>
    <td>332.13</td>
    <td>2.07x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNet18 </td>
    <td>FX</td>
    <td>69.54%</td>
    <td>69.76%</td>
    <td>-0.31%</td>
    <td>611.36</td>
    <td>333.27</td>
    <td>1.83x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNet50</td>
    <td>EAGER</td>
    <td>75.98%</td>
    <td>76.15%</td>
    <td>-0.21%</td>
    <td>327.14</td>
    <td>162.46</td>
    <td>2.01x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNeXt101_32x8d</td>
    <td>EAGER</td>
    <td>79.08%</td>
    <td>79.31%</td>
    <td>-0.29%</td>
    <td>175.93</td>
    <td>61.09</td>
    <td>2.88x</td>
  </tr>
  <tr>
    <td class="tg-zk71">Roberta Base MRPC</td>
    <td>EAGER</td>
    <td>88.25%</td>
    <td>88.18%</td>
    <td>0.08%</td>
    <td>197.96</td>
    <td>99.35</td>
    <td>1.99x</td>
  </tr>
  <tr>
    <td class="tg-zk71">Se_ResNeXt50_32x4d</td>
    <td>EAGER</td>
    <td>78.98%</td>
    <td>79.08%</td>
    <td>-0.13%</td>
    <td>308.19</td>
    <td>144.6</td>
    <td>2.13x</td>
  </tr>
  <tr>
    <td>SqueezeBERT MRPC</td>
    <td>EAGER</td>
    <td>86.87%</td>
    <td>87.65%</td>
    <td>-0.89%</td>
    <td>186.26</td>
    <td>155.67</td>
    <td>1.20x</td>
  </tr>
  <tr>
    <td>SSD ResNet 34</td>
    <td>FX</td>
    <td>19.52</td>
    <td>19.63</td>
    <td>-0.59%</td>
    <td>19.09</td>
    <td>6.88</td>
    <td>2.78x</td>
  </tr>
  <tr>
    <td>Transfo-xl MRPC</td>
    <td>EAGER</td>
    <td>81.97%</td>
    <td>81.20%</td>
    <td>0.94%</td>
    <td>9.65</td>
    <td>7.06</td>
    <td>1.37x</td>
  </tr>
  <tr>
    <td>Wave2Vec2</td>
    <td>FX</td>
    <td>95.71%</td>
    <td>96.60%</td>
    <td>-0.92%</td>
    <td>23.69</td>
    <td>19.58</td>
    <td>1.21x</td>
  </tr>
  <tr>
    <td>Xlm Roberta base MRPC</td>
    <td>EAGER</td>
    <td>88.03%</td>
    <td>88.62%</td>
    <td>-0.67%</td>
    <td>114.31</td>
    <td>99.34</td>
    <td>1.15x</td>
  </tr>
  <tr>
    <td class="tg-zk71">YOLO V3</td>
    <td>EAGER</td>
    <td>24.60%</td>
    <td>24.54%</td>
    <td>0.21%</td>
    <td>71.81</td>
    <td>31.38</td>
    <td>2.29x</td>
  </tr>
</tbody>
</table>

### PyTorch models with Torch 1.12.1+cpu in QAT mode

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th rowspan="2">Example</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput (samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Acc Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td class="tg-zk71">ResNet18</td>
    <td>EAGER</td>
    <td>69.84%</td>
    <td>69.76%</td>
    <td>0.11%</td>
    <td>690.73</td>
    <td>330.85</td>
    <td>2.09x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNet18</td>
    <td>FX</td>
    <td>69.74%</td>
    <td>69.76%</td>
    <td>-0.03%</td>
    <td>614.83</td>
    <td>334.35</td>
    <td>1.84x</td>
  </tr>
  <tr>
    <td>BERT base MRPC QAT</td>
    <td>FX</td>
    <td>89.70%</td>
    <td>89.46%</td>
    <td>0.27%</td>
    <td>127.45</td>
    <td>82.68</td>
    <td>1.54x</td>
  </tr>
  <tr>
    <td class="tg-zk71">ResNet50</td>
    <td>EAGER</td>
    <td>76.05%</td>
    <td>76.15%</td>
    <td>-0.13%</td>
    <td>410.44</td>
    <td>168.81</td>
    <td>2.43x</td>
  </tr>
</tbody>
</table>

### PyTorch models with Torch 1.11.0+cpu IPEX

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th rowspan="2">Example</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput (samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Acc Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td>bert-large-uncased-whole-word-masking-finetuned-squad </td>
    <td>IPEX</td>
    <td>92.9</td>
    <td>93.16</td>
    <td>-0.28%</td>
    <td>31.35</td>
    <td>9.97</td>
    <td>3.14x</td>
  </tr>
  <tr>
    <td>ResNeXt101_32x16d_wsl</td>
    <td>IPEX</td>
    <td>69.48%</td>
    <td>69.76%</td>
    <td>-0.40%</td>
    <td>1189.15</td>
    <td>680</td>
    <td>1.75x</td>
  </tr>
  <tr>
    <td>ResNet50</td>
    <td>IPEX</td>
    <td>76.07%</td>
    <td>76.15%</td>
    <td>-0.10%</td>
    <td>677.69</td>
    <td>381.59</td>
    <td>1.78x</td>
  </tr>
  <tr>
    <td>SSD ResNet34</td>
    <td>IPEX</td>
    <td>19.95%</td>
    <td>20.00%</td>
    <td>-0.25%</td>
    <td>24.07</td>
    <td>6.71</td>
    <td>3.59x</td>
  </tr>
  <tr>
    <td>DistilBERT base MRPC</td>
    <td>IPEX</td>
    <td>86</td>
    <td>86.84</td>
    <td>-0.96%</td>
    <td>98.02</td>
    <td>62.4</td>
    <td>1.57x</td>
  </tr>
</tbody>
</table>

### ONNX Models with ONNX Runtime 1.12.1

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th rowspan="2">Example</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput(samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Acc Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td>AlexNet</td>
    <td>QLinear</td>
    <td>54.73%</td>
    <td>54.79%</td>
    <td>-0.11%</td>
    <td>960.18</td>
    <td>469.17</td>
    <td>2.05x</td>
  </tr>
  <tr>
    <td>AlexNet </td>
    <td>QDQ</td>
    <td>54.71%</td>
    <td>54.79%</td>
    <td>-0.15%</td>
    <td>962.71</td>
    <td>466.56</td>
    <td>2.06x</td>
  </tr>
  <tr>
    <td>ArcFace</td>
    <td>QLinear</td>
    <td>99.80%</td>
    <td>99.80%</td>
    <td>0.00%</td>
    <td>235.14</td>
    <td>130</td>
    <td>1.81x</td>
  </tr>
  <tr>
    <td>BERT base MRPC DYNAMIC</td>
    <td>QLinear</td>
    <td>85.29%</td>
    <td>86.03%</td>
    <td>-0.86%</td>
    <td>294.05</td>
    <td>125.85</td>
    <td>2.34x</td>
  </tr>
  <tr>
    <td>BERT base MRPC STATIC</td>
    <td>QLinear</td>
    <td>85.29%</td>
    <td>86.03%</td>
    <td>-0.86%</td>
    <td>604.07</td>
    <td>256.93</td>
    <td>2.35x</td>
  </tr>
  <tr>
    <td>BERT SQuAD</td>
    <td>QLinear</td>
    <td>80.44</td>
    <td>80.67</td>
    <td>-0.29%</td>
    <td>93.21</td>
    <td>51.45</td>
    <td>1.81x</td>
  </tr>
  <tr>
    <td>BERT SQuAD</td>
    <td>QDQ</td>
    <td>80.44</td>
    <td>80.67</td>
    <td>-0.29%</td>
    <td>93.27</td>
    <td>51.67</td>
    <td>1.80x</td>
  </tr>
  <tr>
    <td>CaffeNet</td>
    <td>QLinear</td>
    <td>56.21%</td>
    <td>56.30%</td>
    <td>-0.16%</td>
    <td>1501.21</td>
    <td>536.1</td>
    <td>2.80x</td>
  </tr>
  <tr>
    <td>CaffeNet</td>
    <td>QDQ</td>
    <td>56.25%</td>
    <td>56.30%</td>
    <td>-0.09%</td>
    <td>1493.36</td>
    <td>533.09</td>
    <td>2.80x</td>
  </tr>
  <tr>
    <td>DistilBERT base MRPC</td>
    <td>QLinear</td>
    <td>84.80%</td>
    <td>84.56%</td>
    <td>0.28%</td>
    <td>1372.84</td>
    <td>485.95</td>
    <td>2.83x</td>
  </tr>
  <tr>
    <td>DistilBERT base MRPC</td>
    <td>QDQ</td>
    <td>84.56%</td>
    <td>84.56%</td>
    <td>0.00%</td>
    <td>541.43</td>
    <td>480.25</td>
    <td>1.13x</td>
  </tr>
  <tr>
    <td>EfficientNet</td>
    <td>QLinear</td>
    <td>77.57%</td>
    <td>77.70%</td>
    <td>-0.17%</td>
    <td>1250.63</td>
    <td>753.09</td>
    <td>1.66x</td>
  </tr>
  <tr>
    <td>EfficientNet</td>
    <td>QDQ</td>
    <td>77.61%</td>
    <td>77.70%</td>
    <td>-0.12%</td>
    <td>1130.67</td>
    <td>748.12</td>
    <td>1.51x</td>
  </tr>
  <tr>
    <td>Emotion Ferplus</td>
    <td>QLinear</td>
    <td>7.86%</td>
    <td>8.00%</td>
    <td>-1.75%</td>
    <td>336.52</td>
    <td>163.72</td>
    <td>2.06x</td>
  </tr>
  <tr>
    <td>Faster R-CNN</td>
    <td>QLinear</td>
    <td>34.05%</td>
    <td>34.37%</td>
    <td>-0.93%</td>
    <td>16.36</td>
    <td>6.18</td>
    <td>2.65x</td>
  </tr>
  <tr>
    <td>Faster R-CNN</td>
    <td>QDQ</td>
    <td>33.97%</td>
    <td>34.37%</td>
    <td>-1.16%</td>
    <td>10.26</td>
    <td>6.18</td>
    <td>1.66x</td>
  </tr>
  <tr>
    <td>FCN</td>
    <td>QLinear</td>
    <td>64.54%</td>
    <td>64.98%</td>
    <td>-0.67%</td>
    <td>40.05</td>
    <td>12.08</td>
    <td>3.31x</td>
  </tr>
  <tr>
    <td>FCN QDQ</td>
    <td>QDQ</td>
    <td>64.65%</td>
    <td>64.98%</td>
    <td>-0.50%</td>
    <td>26.73</td>
    <td>12.04</td>
    <td>2.22x</td>
  </tr>
  <tr>
    <td>GoogleNet</td>
    <td>QLinear</td>
    <td>67.71%</td>
    <td>67.79%</td>
    <td>-0.12%</td>
    <td>740.16</td>
    <td>587.54</td>
    <td>1.26x</td>
  </tr>
  <tr>
    <td>GoogleNet</td>
    <td>QDQ</td>
    <td>67.73%</td>
    <td>67.79%</td>
    <td>-0.09%</td>
    <td>770.51</td>
    <td>567.88</td>
    <td>1.36x</td>
  </tr>
  <tr>
    <td>Inception V1</td>
    <td>QLinear</td>
    <td>67.21%</td>
    <td>67.24%</td>
    <td>-0.04%</td>
    <td>824.15</td>
    <td>601.92</td>
    <td>1.37x</td>
  </tr>
  <tr>
    <td>Inception V1</td>
    <td>QDQ</td>
    <td>67.21%</td>
    <td>67.24%</td>
    <td>-0.04%</td>
    <td>819.85</td>
    <td>597.46</td>
    <td>1.37x</td>
  </tr>
  <tr>
    <td>Mask R-CNN</td>
    <td>QLinear</td>
    <td>33.41%</td>
    <td>33.72%</td>
    <td>-0.92%</td>
    <td>14.18</td>
    <td>5.78</td>
    <td>2.45x</td>
  </tr>
  <tr>
    <td>Mask R-CNN</td>
    <td>QDQ</td>
    <td>33.30%</td>
    <td>33.72%</td>
    <td>-1.25%</td>
    <td>9.42</td>
    <td>5.7</td>
    <td>1.65x</td>
  </tr>
  <tr>
    <td>Mobile bert MRPC</td>
    <td>QLinear</td>
    <td>86.27%</td>
    <td>86.27%</td>
    <td>0.00%</td>
    <td>613.72</td>
    <td>506.41</td>
    <td>1.21x</td>
  </tr>
  <tr>
    <td>MobileBERT SQuAD MLPerf</td>
    <td>QLinear</td>
    <td>89.82</td>
    <td>90.03</td>
    <td>-0.23%</td>
    <td>88.41</td>
    <td>76.07</td>
    <td>1.16x</td>
  </tr>
  <tr>
    <td>MobileNet V2</td>
    <td>QLinear</td>
    <td>65.59%</td>
    <td>66.89%</td>
    <td>-1.94%</td>
    <td>2454.53</td>
    <td>1543.79</td>
    <td>1.59x</td>
  </tr>
  <tr>
    <td>MobileNet V2</td>
    <td>QDQ</td>
    <td>65.82%</td>
    <td>66.89%</td>
    <td>-1.60%</td>
    <td>2164.97</td>
    <td>1564.21</td>
    <td>1.38x</td>
  </tr>
  <tr>
    <td>MobileNet V3 MLPerf</td>
    <td>QLinear</td>
    <td>75.58%</td>
    <td>75.74%</td>
    <td>-0.21%</td>
    <td>2147.42</td>
    <td>1046.69</td>
    <td>2.05x</td>
  </tr>
  <tr>
    <td>MobileNet V3 MLPerf</td>
    <td>QDQ</td>
    <td>75.57%</td>
    <td>75.74%</td>
    <td>-0.22%</td>
    <td>1877.1</td>
    <td>1054.88</td>
    <td>1.78x</td>
  </tr>
  <tr>
    <td>MobileNetV2 (ONNX Model Zoo)</td>
    <td>QLinear</td>
    <td>68.38%</td>
    <td>69.48%</td>
    <td>-1.58%</td>
    <td>2751.7</td>
    <td>1797.64</td>
    <td>1.53x</td>
  </tr>
  <tr>
    <td>MobileNetV2 (ONNX Model Zoo)</td>
    <td>QDQ</td>
    <td>68.51%</td>
    <td>69.48%</td>
    <td>-1.40%</td>
    <td>2656.23</td>
    <td>1835.74</td>
    <td>1.45x</td>
  </tr>
  <tr>
    <td>ResNet50 v1.5 MLPerf</td>
    <td>QLinear</td>
    <td>0.7615</td>
    <td>0.7646</td>
    <td>-0.41%</td>
    <td>764.901</td>
    <td>434.141</td>
    <td>1.76x</td>
  </tr>
  <tr>
    <td>ResNet50 v1.5 MLPerf</td>
    <td>QDQ</td>
    <td>0.7614</td>
    <td>0.7646</td>
    <td>-0.42%</td>
    <td>575.952</td>
    <td>433.75</td>
    <td>1.33x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.5</td>
    <td>QLinear</td>
    <td>0.7226</td>
    <td>0.7229</td>
    <td>-0.04%</td>
    <td>761.12</td>
    <td>432.615</td>
    <td>1.76x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.5</td>
    <td>QDQ</td>
    <td>0.722</td>
    <td>0.7229</td>
    <td>-0.12%</td>
    <td>575.032</td>
    <td>432.894</td>
    <td>1.33x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.5 (ONNX Model Zoo)</td>
    <td>QLinear</td>
    <td>74.81%</td>
    <td>74.99%</td>
    <td>-0.24%</td>
    <td>885.64</td>
    <td>454.02</td>
    <td>1.95x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.5 (ONNX Model Zoo)</td>
    <td>QDQ</td>
    <td>74.76%</td>
    <td>74.99%</td>
    <td>-0.31%</td>
    <td>603.72</td>
    <td>455.86</td>
    <td>1.32x</td>
  </tr>
  <tr>
    <td class="tg-zk71">Roberta Base MRPC</td>
    <td>QLinear</td>
    <td>89.71%</td>
    <td>89.95%</td>
    <td>-0.27%</td>
    <td>644.636</td>
    <td>254.791</td>
    <td>2.53x</td>
  </tr>
  <tr>
    <td>ShuffleNet V2</td>
    <td>QLinear</td>
    <td>66.13%</td>
    <td>66.36%</td>
    <td>-0.35%</td>
    <td>2298.55</td>
    <td>1480.87</td>
    <td>1.55x</td>
  </tr>
  <tr>
    <td>ShuffleNet V2</td>
    <td>QDQ</td>
    <td>66.12%</td>
    <td>66.36%</td>
    <td>-0.36%</td>
    <td>1951.11</td>
    <td>1490.78</td>
    <td>1.31x</td>
  </tr>
  <tr>
    <td>SqueezeNet</td>
    <td>QLinear</td>
    <td>56.54%</td>
    <td>56.87%</td>
    <td>-0.58%</td>
    <td>2588.97</td>
    <td>1605.92</td>
    <td>1.61x</td>
  </tr>
  <tr>
    <td>SqueezeNet</td>
    <td>QDQ</td>
    <td>56.54%</td>
    <td>56.87%</td>
    <td>-0.58%</td>
    <td>2566.18</td>
    <td>1936.79</td>
    <td>1.32x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1</td>
    <td>QLinear</td>
    <td>22.45%</td>
    <td>23.10%</td>
    <td>-2.81%</td>
    <td>725.83</td>
    <td>570.24</td>
    <td>1.27x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1</td>
    <td>QDQ</td>
    <td>22.45%</td>
    <td>23.10%</td>
    <td>-2.81%</td>
    <td>666.01</td>
    <td>539.77</td>
    <td>1.23x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1 (ONNX Model Zoo)</td>
    <td>QLinear</td>
    <td>22.86%</td>
    <td>23.03%</td>
    <td>-0.74%</td>
    <td>641.56</td>
    <td>519.93</td>
    <td>1.23x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1 (ONNX Model Zoo)</td>
    <td>QDQ</td>
    <td>22.86%</td>
    <td>23.03%</td>
    <td>-0.74%</td>
    <td>633.61</td>
    <td>492.5</td>
    <td>1.29x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V2</td>
    <td>QLinear</td>
    <td>24.04%</td>
    <td>24.68%</td>
    <td>-2.59%</td>
    <td>542.68</td>
    <td>401.56</td>
    <td>1.35x</td>
  </tr>
  <tr>
    <td>SSD</td>
    <td>QLinear</td>
    <td>18.84%</td>
    <td>18.98%</td>
    <td>-0.74%</td>
    <td>31.33</td>
    <td>8.87</td>
    <td>3.53x</td>
  </tr>
  <tr>
    <td>SSD</td>
    <td>QDQ</td>
    <td>18.63%</td>
    <td>18.98%</td>
    <td>-1.84%</td>
    <td>23.98</td>
    <td>8.95</td>
    <td>2.68x</td>
  </tr>
  <tr>
    <td>Tiny YOLOv3</td>
    <td>QLinear</td>
    <td>12.08%</td>
    <td>12.43%</td>
    <td>-2.82%</td>
    <td>648.62</td>
    <td>518.97</td>
    <td>1.25x</td>
  </tr>
  <tr>
    <td>VGG16</td>
    <td>QLinear</td>
    <td>66.67%</td>
    <td>66.69%</td>
    <td>-0.03%</td>
    <td>221.93</td>
    <td>99.51</td>
    <td>2.23x</td>
  </tr>
  <tr>
    <td>VGG16 (ONNX Model Zoo)</td>
    <td>QLinear</td>
    <td>72.32%</td>
    <td>72.40%</td>
    <td>-0.11%</td>
    <td>319.54</td>
    <td>99.9</td>
    <td>3.20x</td>
  </tr>
  <tr>
    <td>VGG16 (ONNX Model Zoo)</td>
    <td>QDQ</td>
    <td>72.31%</td>
    <td>72.40%</td>
    <td>-0.12%</td>
    <td>319.41</td>
    <td>99.94</td>
    <td>3.20x</td>
  </tr>
  <tr>
    <td>VGG16</td>
    <td>QDQ</td>
    <td>66.69%</td>
    <td>66.69%</td>
    <td>0.00%</td>
    <td>307.52</td>
    <td>99.24</td>
    <td>3.10x</td>
  </tr>
  <tr>
    <td>YOLOv3</td>
    <td>QLinear</td>
    <td>26.82%</td>
    <td>28.74%</td>
    <td>-6.68%</td>
    <td>124.24</td>
    <td>54.03</td>
    <td>2.30x</td>
  </tr>
  <tr>
    <td>YOLOv4</td>
    <td>QLinear</td>
    <td>33.25%</td>
    <td>33.71%</td>
    <td>-1.36%</td>
    <td>49.76</td>
    <td>32.99</td>
    <td>1.51x</td>
  </tr>
  <tr>
    <td>ZFNet</td>
    <td>QLinear</td>
    <td>55.84%</td>
    <td>55.96%</td>
    <td>-0.21%</td>
    <td>459.38</td>
    <td>261.93</td>
    <td>1.75x</td>
  </tr>
  <tr>
    <td>ZFNet</td>
    <td>QDQ</td>
    <td>55.86%</td>
    <td>55.96%</td>
    <td>-0.18%</td>
    <td>460.66</td>
    <td>264.34</td>
    <td>1.74x</td>
  </tr>
</tbody>
</table>

### MXNet models with MXNet 1.7.0

<table class="tg">
<thead>
  <tr>
    <th rowspan="2">Model</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance<br>Throughput(samples/sec) <br></th>
  </tr>
  <tr>
    <th>INT8</th>
    <th>FP32</th>
    <th>Acc Ratio[(INT8-FP32)/FP32]</th>
    <th>INT8</th>
    <th>FP32</th>
    <th>Performance Ratio[INT8/FP32]</th>
  </tr>
</thead>
<tbody align="center">
  <tr>
    <td>Inception V3</td>
    <td>77.80%</td>
    <td>77.65%</td>
    <td>0.20%</td>
    <td>86.52</td>
    <td>47.98</td>
    <td>1.80x</td>
  </tr>
  <tr>
    <td>MobileNet V1</td>
    <td>71.60%</td>
    <td>72.23%</td>
    <td>-0.86%</td>
    <td>441.59</td>
    <td>337.52</td>
    <td>1.31x</td>
  </tr>
  <tr>
    <td>MobileNet V3 MLPerf</td>
    <td>70.80%</td>
    <td>70.87%</td>
    <td>-0.10%</td>
    <td>272.87</td>
    <td>211.51</td>
    <td>1.29x</td>
  </tr>
  <tr>
    <td>ResNet v1 152</td>
    <td>78.28%</td>
    <td>78.54%</td>
    <td>-0.33%</td>
    <td>65.2</td>
    <td>37.05</td>
    <td>1.76x</td>
  </tr>
  <tr>
    <td>ResNet18 V1.0</td>
    <td>70.01%</td>
    <td>70.14%</td>
    <td>-0.19%</td>
    <td>423.98</td>
    <td>235.98</td>
    <td>1.80x</td>
  </tr>
  <tr>
    <td>ResNet50 V1.0</td>
    <td>75.91%</td>
    <td>76.33%</td>
    <td>-0.55%</td>
    <td>180.69</td>
    <td>100.49</td>
    <td>1.80x</td>
  </tr>
  <tr>
    <td>SqueezeNet</td>
    <td>56.80%</td>
    <td>56.97%</td>
    <td>-0.28%</td>
    <td>311.23</td>
    <td>198.61</td>
    <td>1.57x</td>
  </tr>
  <tr>
    <td>SSD MobileNet V1</td>
    <td>74.94%</td>
    <td>75.54%</td>
    <td>-0.79%</td>
    <td>43.5</td>
    <td>25.77</td>
    <td>1.69x</td>
  </tr>
  <tr>
    <td>SSD ResNet50 V1.0</td>
    <td>80.21%</td>
    <td>80.23%</td>
    <td>-0.03%</td>
    <td>31.64</td>
    <td>15.13</td>
    <td>2.09x</td>
  </tr>
</tbody>
</table>

## Validated Pruning Examples
<table class="docutils">
<thead>
  <tr>
    <th rowspan="2">Tasks</th>
    <th rowspan="2">Framework</th>
    <th rowspan="2">Model</th>
    <th rowspan="2">FP32 Baseline</th>
    <th colspan="3">Gradient Sensitivity with 20% Sparsity</th>
    <th colspan="3">+ONNX Dynamic Quantization on Pruned Model</th>
  </tr>
  <tr>
    <td>Accuracy%</td>
    <td>Drop</td>
    <td>Perf Gain (sample/s)</td>
    <td>Accuracy%</td>
    <td>Drop</td>
    <td>Perf Gain (sample/s)</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>SST-2</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>accuracy = 92.32</td>
    <td>accuracy = 91.97</td>
    <td>-0.38</td>
    <td>1.30x</td>
    <td>accuracy = 92.20</td>
    <td>-0.13</td>
    <td>1.86x</td>
  </tr>
  <tr>
    <td>QQP</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>[accuracy, f1] = [91.10, 88.05]</td>
    <td>[accuracy, f1] = [89.97, 86.54]</td>
    <td>[-1.24, -1.71]</td>
    <td>1.32x</td>
    <td>[accuracy, f1] = [89.75, 86.60]</td>
    <td>[-1.48, -1.65]</td>
    <td>1.81x</td>
  </tr>
</tbody>
</table>

<table class="docutils">
<thead>
  <tr>
    <th rowspan="2">Tasks</th>
    <th rowspan="2">Framework</th>
    <th rowspan="2">Model</th>
    <th rowspan="2">FP32 Baseline</th>
    <th colspan="2">Pattern Lock on 70% Unstructured Sparsity</th>
    <th colspan="2">Pattern Lock on 50% 1:2 Structured Sparsity</th>
  </tr>
  <tr>
    <td>Accuracy%</td>
    <td>Drop</td>
    <td>Accuracy%</td>
    <td>Drop</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>MNLI</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>[m, mm] = [84.57, 84.79]</td>
    <td>[m, mm] = [82.45, 83.27]</td>
    <td>[-2.51, -1.80]</td>
    <td>[m, mm] = [83.20, 84.11]</td>
    <td>[-1.62, -0.80]</td>
  </tr>
  <tr>
    <td>SST-2</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>accuracy = 92.32</td>
    <td>accuracy = 91.51</td>
    <td>-0.88</td>
    <td>accuracy = 92.20</td>
    <td>-0.13</td>
  </tr>
  <tr>
    <td>QQP</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>[accuracy, f1] = [91.10, 88.05]</td>
    <td>[accuracy, f1] = [90.48, 87.06]</td>
    <td>[-0.68, -1.12]</td>
    <td>[accuracy, f1] = [90.92, 87.78]</td>
    <td>[-0.20, -0.31]</td>
  </tr>
  <tr>
    <td>QNLI</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>accuracy = 91.54</td>
    <td>accuracy = 90.39</td>
    <td>-1.26</td>
    <td>accuracy = 90.87</td>
    <td>-0.73</td>
  </tr>
  <tr>
    <td>QnA</td>
    <td>PyTorch</td>
    <td>BERT base</td>
    <td>[em, f1] = [79.34, 87.10]</td>
    <td>[em, f1] = [77.27, 85.75]</td>
    <td>[-2.61, -1.54]</td>
    <td>[em, f1] = [78.03, 86.50]</td>
    <td>[-1.65, -0.69]</td>
  </tr>
</tbody>
</table>

<table class="docutils">
<thead>
  <tr>
    <th>Framework</th>
    <th>Model</th>
    <th>FP32 Baseline</th>
    <th>Compression</th>
    <th>Dataset</th>
    <th>Accuracy% (Drop)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>PyTorch</td>
    <td>ResNet18</td>
    <td>69.76</td>
    <td>30% Sparsity on Magnitude</td>
    <td>ImageNet</td>
    <td>69.47(-0.42)</td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>ResNet18</td>
    <td>69.76</td>
    <td>30% Sparsity on Gradient Sensitivity</td>
    <td>ImageNet</td>
    <td>68.85(-1.30)</td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>ResNet50</td>
    <td>76.13</td>
    <td>30% Sparsity on Magnitude</td>
    <td>ImageNet</td>
    <td>76.11(-0.03)</td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>ResNet50</td>
    <td>76.13</td>
    <td>30% Sparsity on Magnitude and Post Training Quantization</td>
    <td>ImageNet</td>
    <td>76.01(-0.16)</td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>ResNet50</td>
    <td>76.13</td>
    <td>30% Sparsity on Magnitude and Quantization Aware Training</td>
    <td>ImageNet</td>
    <td>75.90(-0.30)</td>
  </tr>
</tbody>
</table>

## Validated Knowledge Distillation Examples
<table class="docutils">
<thead>
  <tr>
    <th rowspan="2">Example Name</th>
    <th rowspan="2">Dataset</th>
    <th rowspan="2">Student<br>(Accuracy)</th>
    <th rowspan="2">Teacher<br>(Accuracy)</th>
    <th rowspan="2">Student With Distillation<br>(Accuracy Improvement)</th>
  </tr>
  <tr>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="2">ResNet example</td>
    <td rowspan="2">ImageNet</td>
    <td rowspan="2">ResNet18<br>(0.6739)</td>
    <td rowspan="2">ResNet50<br>(0.7399)</td>
    <td rowspan="2">0.6845<br>(0.0106)</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td rowspan="2">BlendCNN example</td>
    <td rowspan="2">MRPC</td>
    <td rowspan="2">BlendCNN<br>(0.7034)</td>
    <td rowspan="2">BERT-Base<br>(0.8382)</td>
    <td rowspan="2">0.7034<br>(0)</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td rowspan="2">BiLSTM example</td>
    <td rowspan="2">SST-2</td>
    <td rowspan="2">BiLSTM<br>(0.7913)</td>
    <td rowspan="2">RoBERTa-Base<br>(0.9404)</td>
    <td rowspan="2">0.8085<br>(0.0172)</td>
  </tr>
  <tr>
  </tr>
</tbody>
</table>

## Validated ONNX QDQ INT8 models on multiple hardware through ONNX Runtime

<table class="tg">
<thead>
  <tr>
    <th class="tg-y3we">Model (ONNX QDQ)</th>
    <th class="tg-pm1l">AWS c6i.2xlarge<br>INTEL</th>
    <th class="tg-pm1l">AWS c6a.2xlarge<br>AMD</th>
    <th class="tg-pm1l">AWS c6g.2xlarge<br>ARM</th>
    <th class="tg-8d8j">NV A100 CUDA<br>Execution Provider</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-cwad">ResNet50</td>
    <td class="tg-pm1l">74.76%</td>
    <td class="tg-pm1l">68.95%</td>
    <td class="tg-pm1l">74.76%</td>
    <td class="tg-413a">74%</td>
  </tr>
  <tr>
    <td class="tg-cwad">BERT-base</td>
    <td class="tg-pm1l">85.54%</td>
    <td class="tg-pm1l">84.56%</td>
    <td class="tg-pm1l">85.54%</td>
    <td class="tg-413a">85%</td>
  </tr>
  <tr>
    <td class="tg-cwad">ResNet50 V1.5</td>
    <td class="tg-pm1l">72.20%</td>
    <td class="tg-pm1l">67.70%</td>
    <td class="tg-pm1l">72.20%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">MobileNet V2</td>
    <td class="tg-pm1l">65.82%</td>
    <td class="tg-pm1l">58.56%</td>
    <td class="tg-pm1l">65.83%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">SSD MobileNet V1</td>
    <td class="tg-pm1l">22.45%</td>
    <td class="tg-pm1l">16.53%</td>
    <td class="tg-pm1l">22.45%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">DistilBERT base MRPC</td>
    <td class="tg-pm1l">84.56%</td>
    <td class="tg-pm1l">83.82%</td>
    <td class="tg-pm1l">84.56%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">SqueezeNet</td>
    <td class="tg-pm1l">56.54%</td>
    <td class="tg-pm1l">53.52%</td>
    <td class="tg-pm1l">56.54%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">SSD</td>
    <td class="tg-pm1l">18.63%</td>
    <td class="tg-pm1l">18.54%</td>
    <td class="tg-pm1l">18.63%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">AlexNet</td>
    <td class="tg-pm1l">54.71%</td>
    <td class="tg-pm1l">47.06%</td>
    <td class="tg-pm1l">54.71%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">CaffeNet</td>
    <td class="tg-pm1l">56.25%</td>
    <td class="tg-pm1l">52.35%</td>
    <td class="tg-pm1l">56.27%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">GoogleNet</td>
    <td class="tg-pm1l">67.73%</td>
    <td class="tg-pm1l">63.56%</td>
    <td class="tg-pm1l">67.72%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">ZFNet</td>
    <td class="tg-pm1l">55.86%</td>
    <td class="tg-pm1l">45.09%</td>
    <td class="tg-pm1l">55.86%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">Inception V1</td>
    <td class="tg-pm1l">67.21%</td>
    <td class="tg-pm1l">63.03%</td>
    <td class="tg-pm1l">67.20%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">SSD MobileNet V1 (ONNX Model Zoo)</td>
    <td class="tg-pm1l">22.86%</td>
    <td class="tg-pm1l">16.94%</td>
    <td class="tg-pm1l">22.80%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">Mobile bert MRPC</td>
    <td class="tg-pm1l">85.54%</td>
    <td class="tg-pm1l">84.56%</td>
    <td class="tg-pm1l">85.54%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">Roberta base MRPC</td>
    <td class="tg-pm1l">89.46%</td>
    <td class="tg-pm1l">90.44%</td>
    <td class="tg-pm1l">89.71%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">ResNet50 V1.5 MLPerf</td>
    <td class="tg-pm1l">76.14%</td>
    <td class="tg-pm1l">72.80%</td>
    <td class="tg-pm1l">76.14%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">VGG16</td>
    <td class="tg-pm1l">66.69%</td>
    <td class="tg-pm1l">64.25%</td>
    <td class="tg-pm1l">66.69%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">VGG16 (ONNX Model Zoo)</td>
    <td class="tg-pm1l">72.31%</td>
    <td class="tg-pm1l">69.35%</td>
    <td class="tg-pm1l">72.32%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">MobileNet V3 MLPerf</td>
    <td class="tg-pm1l">75.57%</td>
    <td class="tg-pm1l">70.78%</td>
    <td class="tg-pm1l">75.56%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">EfficientNet</td>
    <td class="tg-pm1l">77.61%</td>
    <td class="tg-pm1l">76.52%</td>
    <td class="tg-pm1l">77.56%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-cwad">MobileNet V2 (ONNX Model Zoo)</td>
    <td class="tg-pm1l">68.51%</td>
    <td class="tg-pm1l">62.48%</td>
    <td class="tg-pm1l">68.58%</td>
    <td class="tg-8d8j">*</td>
  </tr>
  <tr>
    <td class="tg-413a">ShuffleNet V2</td>
    <td class="tg-pm1l">66.12%</td>
    <td class="tg-pm1l">58.41%</td>
    <td class="tg-pm1l">66.11%</td>
    <td class="tg-8d8j">*</td>
  </tr>
</tbody>
</table>

> **Note:**
> More NVidia A100 cases test in progress.
