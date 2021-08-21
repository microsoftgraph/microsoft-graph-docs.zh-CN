---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffcda19558951e1fec433d75a58a99a69c57ff55225918995fb0f0c13b81d1ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219753"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest"]]];
[urlRequest setHTTPMethod:@"POST"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```