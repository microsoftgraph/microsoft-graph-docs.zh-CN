---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a42958399b0e80a6a20b5a44b033aec69c3436f9
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559713"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/{caseId}/settings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryCaseSettings *caseSettings = [[MSGraphEdiscoveryCaseSettings alloc] init];
MSGraphEdiscoveryRedundancyDetectionSettings *redundancyDetection = [[MSGraphEdiscoveryRedundancyDetectionSettings alloc] init];
[redundancyDetection setIsEnabled: false];
[redundancyDetection setSimilarityThreshold: 70];
[redundancyDetection setMinWords: 12];
[redundancyDetection setMaxWords: 400000];
[caseSettings setRedundancyDetection:redundancyDetection];
MSGraphEdiscoveryTopicModelingSettings *topicModeling = [[MSGraphEdiscoveryTopicModelingSettings alloc] init];
[topicModeling setIsEnabled: false];
[topicModeling setIgnoreNumbers: false];
[topicModeling setTopicCount: 50];
[topicModeling setDynamicallyAdjustTopicCount: false];
[caseSettings setTopicModeling:topicModeling];
MSGraphEdiscoveryOcrSettings *ocr = [[MSGraphEdiscoveryOcrSettings alloc] init];
[ocr setIsEnabled: true];
[ocr setMaxImageSize: 12000];
[caseSettings setOcr:ocr];

NSError *error;
NSData *caseSettingsData = [caseSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:caseSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```