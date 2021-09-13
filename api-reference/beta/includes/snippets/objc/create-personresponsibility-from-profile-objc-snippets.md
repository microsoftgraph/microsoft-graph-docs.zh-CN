---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2842672a48fd27750305cfcaa72a3745f84104ab4f2a46b35fcfa05fb4b7ae16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106102"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/responsibilities"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphString *string = [[MSGraphString alloc] init];
[string setDescription:@"Member of the Microsoft API Council"];
[string setDisplayName:@"API Council"];
NSMutableArray *collaborationTagsList = [[NSMutableArray alloc] init];
[collaborationTagsList addObject: @"askMeAbout"];
[string setCollaborationTags:collaborationTagsList];

NSError *error;
NSData *stringData = [string getSerializedDataWithError:&error];
[urlRequest setHTTPBody:stringData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```