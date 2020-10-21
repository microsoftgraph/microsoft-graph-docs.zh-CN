---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18004d5a9daee5e70f8f7392fe24bfc84910e38a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609099"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders/{id}/contacts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
[contact setParentFolderId:@"parentFolderId-value"];
[contact setBirthday:@"datetime-value"];
[contact setFileAs:@"fileAs-value"];
[contact setDisplayName:@"displayName-value"];
[contact setGivenName:@"givenName-value"];
[contact setInitials:@"initials-value"];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```