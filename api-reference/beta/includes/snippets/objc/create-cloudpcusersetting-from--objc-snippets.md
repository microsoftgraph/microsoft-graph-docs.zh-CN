---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1aff7a5b0e751438a457f89d45611536907b11b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334210"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/userSettings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcUserSetting *cloudPcUserSetting = [[MSGraphCloudPcUserSetting alloc] init];
[cloudPcUserSetting setDisplayName:@"Example"];
[cloudPcUserSetting setSelfServiceEnabled: false];
[cloudPcUserSetting setLocalAdminEnabled: true];
MSGraphCloudPcRestorePointSetting *restorePointSetting = [[MSGraphCloudPcRestorePointSetting alloc] init];
[restorePointSetting setFrequencyInHours: 16];
[restorePointSetting setUserRestoreEnabled: true];
[cloudPcUserSetting setRestorePointSetting:restorePointSetting];

NSError *error;
NSData *cloudPcUserSettingData = [cloudPcUserSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcUserSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```