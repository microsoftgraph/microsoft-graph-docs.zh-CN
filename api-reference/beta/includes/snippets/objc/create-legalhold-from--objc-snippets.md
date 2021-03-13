---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79442c9ec3069209e6bc45df99fd6613931c1c70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773835"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/{caseId}/legalHolds"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryLegalHold *legalHold = [[MSGraphEdiscoveryLegalHold alloc] init];
[legalHold setDescription:@"String"];
MSGraphIdentitySet *createdBy = [[MSGraphIdentitySet alloc] init];
[legalHold setCreatedBy:createdBy];
[legalHold setIsEnabled:@"Boolean"];
[legalHold setStatus: [MSGraphEdiscoveryLegalHoldStatus Pending]];
[legalHold setContentQuery:@"String"];
NSMutableArray *errorsList = [[NSMutableArray alloc] init];
[errorsList addObject: @"String"];
[legalHold setErrors:errorsList];
[legalHold setDisplayName:@"String"];

NSError *error;
NSData *legalHoldData = [legalHold getSerializedDataWithError:&error];
[urlRequest setHTTPBody:legalHoldData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```