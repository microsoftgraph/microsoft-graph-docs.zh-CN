---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 948f85dc4d2aca20e0b76050e956c9bc4eb65c368bef1dbb20c4ba1ae7836dd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333232"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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