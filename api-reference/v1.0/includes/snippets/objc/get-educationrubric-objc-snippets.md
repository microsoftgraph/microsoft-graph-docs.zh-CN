---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e5579d1c0036b1ec5bcbb239e38c9a5fe30596e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990935"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEducationRubric *educationRubric = [[MSGraphEducationRubric alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```