---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e2bbf3e8043db834d2d27f3e38aa6240389e4bcbe2669e439eaf3fc61bbcbc0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333138"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/masterCategories"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookCategory *outlookCategory = [[MSGraphOutlookCategory alloc] init];
[outlookCategory setDisplayName:@"Project expenses"];
[outlookCategory setColor: [MSGraphCategoryColor preset9]];

NSError *error;
NSData *outlookCategoryData = [outlookCategory getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookCategoryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```