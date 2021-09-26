---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e917c85cb48ba3a5e097879e14bf1ed640fe0bac6ef2c7aa9045e64d0800c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105238"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/onPremisesConnections/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCloudPcOnPremisesConnection *cloudPcOnPremisesConnection = [[MSGraphCloudPcOnPremisesConnection alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```