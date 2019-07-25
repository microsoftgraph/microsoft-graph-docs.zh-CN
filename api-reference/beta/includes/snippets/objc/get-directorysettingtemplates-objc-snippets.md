---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f09899cbfc0f12b8b76c8051563eae7fb84a0764
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706335"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directorySettingTemplates"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directorySettingTemplateList = [[NSMutableArray alloc] init];
        directorySettingTemplateList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectorySettingTemplate *directorySettingTemplate = [[MSGraphDirectorySettingTemplate alloc] initWithDictionary:[directorySettingTemplateList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```