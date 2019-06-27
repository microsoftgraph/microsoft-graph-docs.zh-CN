---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99415b7b729318b5d4cf4f6f27d57843dde2841d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318384"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contactFolders"]]];
[urlRequest setHTTPMethod:@"POST"];
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