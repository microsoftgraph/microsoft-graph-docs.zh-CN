---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 71b2ef704033b431f6737ab3d41c37c0133bff15
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714423"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/synchronizationProfiles/{id}/errors"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *educationSynchronizationErrorList = [[NSMutableArray alloc] init];
        educationSynchronizationErrorList = [jsonFinal valueForKey:@"value"];
        MSGraphEducationSynchronizationError *educationSynchronizationError = [[MSGraphEducationSynchronizationError alloc] initWithDictionary:[educationSynchronizationErrorList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```