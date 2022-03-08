---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 118e5b824d2883b53541c0e648828dbc400e4ff7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338239"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/search/bookmarks/{bookmarksId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSearchBookmark *bookmark = [[MSGraphSearchBookmark alloc] init];
[bookmark setDescription:@"Book a fancy vacation in Tuscany or browse museums in Florence."];

NSError *error;
NSData *bookmarkData = [bookmark getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookmarkData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```