---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fefaabbb057267c8c411df3c0a0f85754642b4f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220284"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/organizationSettings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcOrganizationSettings *cloudPcOrganizationSettings = [[MSGraphCloudPcOrganizationSettings alloc] init];
[cloudPcOrganizationSettings setUserAccountType: [MSGraphCloudPcUserAccountType standardUser]];
[cloudPcOrganizationSettings setOsVersion: [MSGraphCloudPcOperatingSystem windows11]];
MSGraphCloudPcWindowsSettings *windowsSettings = [[MSGraphCloudPcWindowsSettings alloc] init];
[windowsSettings setLanguage:@"en-US"];
[cloudPcOrganizationSettings setWindowsSettings:windowsSettings];

NSError *error;
NSData *cloudPcOrganizationSettingsData = [cloudPcOrganizationSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcOrganizationSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```