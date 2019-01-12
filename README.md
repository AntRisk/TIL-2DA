# CMMN(Counter Malicious Merchant Network)
An implementation of Time-Interval-LSTM with 2D-Attention

## From Paper:
### Introduction
Nowadays, in-store payment through ad-hoc mobile Apps (e.g. Alipay)
becomes prevailing in daily offline consumption environment,
leading to the reform of payment solutions for offline merchants,
meanwhile more illegal trading activities. It is obvious that perceiving
those malicious merchants in registration precisely before
they entering the trading system and conducting real transactions
could achieve the minimum cost. Nonetheless, assessment of latent
malicious offline merchants in registration relies heavily on
expert experience driven rule-based engine, which can be labor intensive
and time consuming. Besides, the inherent cold-start nature
of Alipay offline merchant registration makes it difficult to yield an
accurate prediction.
In this study, we propose a novel event sequence learning model
\- Counter Malicious Merchant Network (CMMN) based on timeinterval-
LSTM with 2D-attention mechanism, in order to detect
malicious Alipay offline merchant in registration at Ant Financial.
CMMN implements an Encoder-Decoder architecture, where an innovative
2D-attention mechanism is developed as the linkage. The
2D-attention mechanism is capable of assigning attention weight of
encoder hidden states in both feature and temporal spaces simultaneously.
Furthermore, we apply a customized time-interval-LSTM
unit that actively simulates the time intervals between neighboring
events, such that the underlying correlation between events
can be explicitly extracted in both short-term and long-term periods.
To tackle the cold-start problem, we introduce the Customer
to Business (C2B) modeling chain that reversely outreaches the
modeling period from the business end to enrich data availability.
An extensive set of offline experiments demonstrate that CMMN
can deliver better forecast performance over other cutting-edge
baseline models. The online test indicates that CMMN augments existing
decision-making practices of Alipay offline merchant access
security check. As a result, the precision and recall rate of malicious
Alipay offline merchant detection in registration are increased by
4.4% and 9.9% respectively on average.
![Architecture](./figs/C2B.jpg)

#### The Architecture of CMMN
![Architecture](./figs/architecture.jpg)

#### The Prototype of Timeinterval-LSTM
![TimeIntervalLSTM](./figs/time_interval_lstm.jpg)
