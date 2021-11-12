---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 132a0fce3f436b6ca2b811a2454b44e4e9e25d948e70c2d72b4334c3084026ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903821"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/settings/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectorySetting *directorySetting = [[MSGraphDirectorySetting alloc] init];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"name-value"];
[values setValue:@"value-value"];
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