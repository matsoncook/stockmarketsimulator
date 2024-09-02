```mermaid
graph TD;
    subgraph Predict and Place
        FutureFixtures[Future Fixtures]
        Predictions[Predictions]
        Place[Place]
    end
    subgraph Backtest
        PredictionParameters[Prediction Parameters]
        Rankings[Rankings]
        PastResults[Past Results]
    end
    FutureFixtures-->Predictions;
    Predictions-->Place;
    Place-->PastResults;
    PredictionParameters-->Predictions;
    PastResults-->Rankings;
    Rankings-->PredictionParameters;
    
    