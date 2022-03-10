---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cdcd0ae761d32a7cb515b4f933c1f6b5194e2a2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411674"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/settings/3c105fc3-2254-4861-9e2d-d59e2126f3ef"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectorySetting *directorySetting = [[MSGraphDirectorySetting alloc] init];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"CustomBlockedWordsList"];
[values setValue:@"Contoso"];
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