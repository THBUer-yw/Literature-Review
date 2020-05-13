# Paper reveiw

* [Machinery health prognostics: A systematic review from data acquisition to RUL prediction](https://www.sciencedirect.com/science/article/abs/pii/S0888327017305988)
  - 2017年RUL的review文章，总结非常到位

## RUL prediction

### 1. AI-based methods

* 2020.01: [A new data-driven transferable remaining useful life prediction approach for bearing under different working conditions]()
  - 使用HMM实现FOT的判断，使用MMD-Based MLP进行了迁移学习，在IEEE 2012 Data Challenge上进行了验证；
  
* 2020.04: [Data alignments in machinery remaining useful life prediction using deep adversarial neural networks]()
  - 使用GAN的方式进行了FOT的构建，同时使用对抗学习的想法进行了迁移，但是并没有特别明确的表明，文章中提到使用了data alignment，在XJTU-SY Dataset 和 PHM 2012 dataset 上进行了验证；
  
* 2020.03: [A novel approach for predicting tool remaining useful life using limited data]()
  - 这篇主要是对milling experiments进行分析，先构建了Adaptive time window，主要用于确定FOT，其内核是Tool wear factor determination，刀具磨损，然后是用Deep bidirectional LSTM进行数据有限条件下的剩余寿命预测，但是具体数据如何有限的条件并不非常明确，在milling machine tool进行了验证（可能是自己的数据集）；
  
  
### 2. Statistical model-based methods


### 3. Hybrid approaches


### 4. Physics model-based approaches

## HI construction

* 2020.01: [A new method for the estimation of bearing health state and remaining useful life based on the moving average
cross-correlation of power spectral density]()
  - 构建了新的Health index, ‘MAC2PSD’, 使用的是滑动平均相关滤波，分了5个阶段，最后使用分阶段的方式进行寿命预测，指标构建的方法缺陷在于最终还是需要专家去确认，使用Case study 1: Rexnord/NASA data 和 Case study 1: Rexnord/NASA data
