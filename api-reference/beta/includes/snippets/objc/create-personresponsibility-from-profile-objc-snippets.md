---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e876652e1665a7ec4ada5c27c1e775158c648126
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440956"
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