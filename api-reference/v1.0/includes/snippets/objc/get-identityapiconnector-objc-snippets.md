---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03d0ca9122394fdcdb7a00f78466c1d8ee453441e5157ef2715dc326da44a394
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904313"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphIdentityApiConnector *identityApiConnector = [[MSGraphIdentityApiConnector alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```