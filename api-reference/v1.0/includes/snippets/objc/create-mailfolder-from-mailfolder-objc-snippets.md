---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b36684703b4e2205b804515b64535ea417e04d2eaa7be3f3973ca471431259a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333215"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/{id}/childFolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailFolder *mailFolder = [[MSGraphMailFolder alloc] init];
[mailFolder setDisplayName:@"displayName-value"];
[mailFolder setIsHidden: true];

NSError *error;
NSData *mailFolderData = [mailFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```