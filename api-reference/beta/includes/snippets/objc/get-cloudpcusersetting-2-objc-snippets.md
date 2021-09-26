---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc4e8e9c789223a09e7ad643f065fbf02061c846b3f47d5ec1cfda6218d1ec5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158380"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphCloudPcUserSetting *cloudPcUserSetting = [[MSGraphCloudPcUserSetting alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```