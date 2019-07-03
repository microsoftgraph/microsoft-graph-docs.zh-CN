---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 47c2ffc252d32109e5d15f619a944a920d43598a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468116"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupSettingTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupSettingTemplateList = [[NSMutableArray alloc] init];
        groupSettingTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphGroupSettingTemplate *groupSettingTemplate = [[MSGraphGroupSettingTemplate alloc] initWithDictionary:[groupSettingTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```