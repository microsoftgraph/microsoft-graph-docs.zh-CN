---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b7a539257aa441510b3d527135a509fda719d3ab68f401729dc222b02fe95a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332406"
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