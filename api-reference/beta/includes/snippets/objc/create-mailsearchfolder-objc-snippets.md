---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb798c0a7a1447e5a69625ff06f7cc63f99c7c9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619489"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailFolder *mailFolder = [[MSGraphMailFolder alloc] init];
[mailFolder setDisplayName:@"Weekly digests"];
[mailFolder setIncludeNestedFolders: true];
NSMutableArray *sourceFolderIdsList = [[NSMutableArray alloc] init];
[sourceFolderIdsList addObject: @"AQMkADYAAAIBDAAAAA=="];
[mailFolder setSourceFolderIds:sourceFolderIdsList];
[mailFolder setFilterQuery:@"contains(subject, 'weekly digest')"];

NSError *error;
NSData *mailFolderData = [mailFolder getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailFolderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```