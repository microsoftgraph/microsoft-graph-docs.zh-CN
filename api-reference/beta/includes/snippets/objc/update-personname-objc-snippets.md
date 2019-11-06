---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 026da245e2d1be835b06275684cb9329d3070df7
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997210"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/names/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonName *personName = [[MSGraphPersonName alloc] init];
[personName setDisplayName:@"displayName-value"];
[personName setFirst:@"first-value"];
[personName setInitials:@"initials-value"];
[personName setLast:@"last-value"];
[personName setLanguageTag:@"languageTag-value"];
[personName setMaiden:@"maiden-value"];

NSError *error;
NSData *personNameData = [personName getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personNameData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```