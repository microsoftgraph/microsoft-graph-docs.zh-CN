---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b2e89f29c5b56bb788a44e6d0c6d0166ec09515
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997787"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/names"]]];
[urlRequest setHTTPMethod:@"POST"];
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