---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 506b74642b16f687356e743bc427cb3d48b785f95c43508b3f5512286f0c00c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278498"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContactFolder *contactFolder = [[MSGraphContactFolder alloc] init];
[contactFolder setParentFolderId:@"parentFolderId-value"];
[contactFolder setDisplayName:@"displayName-value"];

NSError *error;
NSData *contactFolderData = [contactFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```