---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 069edbbc8502b815e589833f095f0c75f33f9fa58a153a45ee7191cb73681241
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904257"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcUserSetting *cloudPcUserSetting = [[MSGraphCloudPcUserSetting alloc] init];
[cloudPcUserSetting setDisplayName:@"Example"];
[cloudPcUserSetting setSelfServiceEnabled: true];
[cloudPcUserSetting setLocalAdminEnabled: false];

NSError *error;
NSData *cloudPcUserSettingData = [cloudPcUserSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcUserSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```