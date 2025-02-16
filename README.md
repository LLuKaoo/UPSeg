# UPSeg
Code Implementation of **UPSeg: Unleashing the Power of Multi-Modal Synergy in Remote Sensing Semantic Segmentation**

## Introduction
<!-- <p><img src="figures/gfm.png" width="1000" /></p> -->
<div align="center">
    <img src="Fig1.png" height="250px" />
</div>
<!-- <img src="gfm.png" width="300"> -->

As multi-modal remote sensing data becomes increasingly accessible, foundation models for multi-modal remote sensing are being developed to align different modalities, enabling the integration of diverse data sources. However, current foundation models often focus primarily on learning shared characteristics across modalities, pushing inherently unrelated representations to converge while overlooking the synergistic information that emerges only through modal interactions. This limitation hinders their ability to advance the comprehensive analysis of Earth observation data. To this end, we propose a novel multi-modal remote sensing semantic segmentation method, UPSeg, to fully explore the intricate interactions across modalities for detailed characteristics of land features. It emulates human cognitive orientation for multi-modal interactions, i.e., information from one modality can stimulate understanding of another, reducing uncertain information arising from a single modality and obtain a comprehensive multi-modal feature representation. Extensive evaluation demonstrates that the proposed algorithm effectively addresses the limitations of existing foundation models in leveraging modal synergies, facilitating precise land cover classification.

## Results
<table>
    <tr>
        <td rowspan="2">Method</td> 
        <td colspan="2">WHU-OPT-SAR</td> 
        <td colspan="2">GID</td> 
   </tr>
    <tr>
  		  <td>mIoU</td> 
        <td>mPA</td> 
        <td>mIoU</td> 
        <td>mPA</td> 
    </tr>
    <tr>
        <td>PAGNet</td> 
        <td>38.6</td> 
        <td>49.3</td> 
        <td>54.6</td> 
        <td>68.9</td> 
    </tr>
    <tr>
        <td>AMMFuse-Net</td> 
        <td>45.2</td> 
        <td>57.1</td> 
        <td>47.9</td> 
        <td>62.6</td> 
    </tr>
    <tr>
        <td>MCANet</td> 
        <td>48.5</td> 
        <td>61.0</td> 
        <td>53.0</td> 
        <td>70.0</td> 
    </tr>
    <tr>
        <td>CMX</td> 
        <td>45.9</td> 
        <td>57.5</td> 
        <td>59.1</td> 
        <td>73.0</td> 
    </tr>
      <tr>
        <td>SSLViT</td> 
        <td>43.1</td> 
        <td>54.2</td> 
        <td>53.7</td> 
        <td>67.5</td> 
    </tr>
    <tr>
        <td>CROMA</td> 
        <td>43.9</td> 
        <td>54.5</td> 
        <td>53.5</td> 
        <td>67.7</td> 
    </tr>
    <tr>
        <td>DeCUR</td> 
        <td>44.3</td> 
        <td>55.6</td> 
        <td>57.4</td> 
        <td>71.1</td> 
    </tr>
    <tr>
        <td>DOFA</td> 
        <td>47.5</td> 
        <td>60.6</td> 
        <td>61.5</td> 
        <td>75.6</td> 
    </tr>
    <tr>
        <td>UPSeg</td> 
        <td>51.3</td> 
        <td>66.5</td> 
        <td>66.5</td> 
        <td>80.3</td> 
    </tr>
</table>

## TODO
- [ ] Refactor code
- [ ] Submit initial version

## Acknowledgment
This repo is based on [DOFA](https://github.com/zhu-xlab/DOFA) which is an excellent work.
