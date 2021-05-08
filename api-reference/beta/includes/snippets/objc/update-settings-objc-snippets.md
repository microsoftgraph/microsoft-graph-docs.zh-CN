---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 894c9841326e7980445324c7ae3c6ffd19d2f367
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240830"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/{caseId}/settings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoverySettings *settings = [[MSGraphEdiscoverySettings alloc] init];
MSGraphEdiscoveryRedundancyDetectionSettings *redundancyDetection = [[MSGraphEdiscoveryRedundancyDetectionSettings alloc] init];
[redundancyDetection setIsEnabled: false];
[redundancyDetection setSimilarityThreshold: 70];
[redundancyDetection setMinWords: 12];
[redundancyDetection setMaxWords: 400000];
[settings setRedundancyDetection:redundancyDetection];
MSGraphEdiscoveryTopicModelingSettings *topicModeling = [[MSGraphEdiscoveryTopicModelingSettings alloc] init];
[topicModeling setIsEnabled: false];
[topicModeling setIgnoreNumbers: false];
[topicModeling setTopicCount: 50];
[topicModeling setDynamicallyAdjustTopicCount: false];
[settings setTopicModeling:topicModeling];
MSGraphEdiscoveryOcrSettings *ocr = [[MSGraphEdiscoveryOcrSettings alloc] init];
[ocr setIsEnabled: true];
[ocr setMaxImageSize: 12000];
[settings setOcr:ocr];

NSError *error;
NSData *settingsData = [settings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:settingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```