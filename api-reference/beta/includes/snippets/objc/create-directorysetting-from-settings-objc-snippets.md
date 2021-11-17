---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49a57a3e9c56b79ebe41ee9186d03fd9969a8e9b
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513038"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/settings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectorySetting *directorySetting = [[MSGraphDirectorySetting alloc] init];
[directorySetting setDisplayName:@"Group.Unified"];
[directorySetting setTemplateId:@"62375ab9-6b52-47ed-826b-58e47e0e304b"];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"GuestUsageGuidelinesUrl"];
[values setValue:@"https://privacy.contoso.com/privacystatement"];
[valuesList addObject: values];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"EnableMSStandardBlockedWords"];
[values setValue:@"true"];
[valuesList addObject: values];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"EnableMIPLabels"];
[values setValue:@"true"];
[valuesList addObject: values];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"PrefixSuffixNamingRequirement"];
[values setValue:@"[Contoso-][GroupName]"];
[valuesList addObject: values];
[directorySetting setValues:valuesList];

NSError *error;
NSData *directorySettingData = [directorySetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:directorySettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```