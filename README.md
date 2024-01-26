List<InterventionRuleSearch> capturedDocuments = null;
searchClientMock.Setup(client => client.UploadDocuments(It.IsAny<List<InterventionRuleSearch>>()))
    .Callback((List<InterventionRuleSearch> documents) => capturedDocuments = documents);
