---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 753cae6f14c2022d81a3806d0bbe2c3d68fa6f7c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395109"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/settings/contactMergeSuggestions"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContactMergeSuggestions *contactMergeSuggestions = [[MSGraphContactMergeSuggestions alloc] init];
[contactMergeSuggestions setIsEnabled: false];

NSError *error;
NSData *contactMergeSuggestionsData = [contactMergeSuggestions getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactMergeSuggestionsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```