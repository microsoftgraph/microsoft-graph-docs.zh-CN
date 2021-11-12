---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3421f2c81636676a62052b8d4b02e24d1b8aa0dc4394315907b8871c18447ada
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218916"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```