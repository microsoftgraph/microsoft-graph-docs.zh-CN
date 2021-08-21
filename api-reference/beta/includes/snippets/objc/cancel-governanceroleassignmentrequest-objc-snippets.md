---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59c21703a82a99ae913ec5af00f2a2f1b1b435bc75f29ea05336ab65e4879a68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161451"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel"]]];
[urlRequest setHTTPMethod:@"POST"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```