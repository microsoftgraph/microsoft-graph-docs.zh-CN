---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bdd8b21fbd4c9e937aadfff3ee8bf670c534a595
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322724"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] init];
[groupSetting setDisplayName:@"displayName-value"];
[groupSetting setTemplateId:@"templateId-value"];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"name-value"];
[values setValue:@"value-value"];
[valuesList addObject: values];
[groupSetting setValues:valuesList];

NSError *error;
NSData *groupSettingData = [groupSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```