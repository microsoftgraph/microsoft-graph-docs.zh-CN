---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8f2d165d1aea14c97a1bf6cc0613f839ff05f79b0267d84254e1b3b8c139979
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332398"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/synchronizationProfiles/{id}/profileStatus"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEducationSynchronizationProfileStatus *educationSynchronizationProfileStatus = [[MSGraphEducationSynchronizationProfileStatus alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```