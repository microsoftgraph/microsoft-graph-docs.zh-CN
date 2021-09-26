---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce9973adbcd1a7d8cfb19880b73d6203d3e45d1ef322d49b694a19f16670258
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158386"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCloudPcUserSetting *cloudPcUserSetting = [[MSGraphCloudPcUserSetting alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```