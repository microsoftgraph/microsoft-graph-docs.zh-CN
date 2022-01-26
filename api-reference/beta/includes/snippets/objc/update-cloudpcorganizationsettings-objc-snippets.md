---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70c86a838ead804031975dad6b33c1f7cd3549c
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225012"
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

NSError *error;
NSData *cloudPcOrganizationSettingsData = [cloudPcOrganizationSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcOrganizationSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```