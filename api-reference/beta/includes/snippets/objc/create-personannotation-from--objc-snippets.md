---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1e25380f06e9de69e855bd21f4a344a1e6e2bd
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820208"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/notes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAnnotation *personAnnotation = [[MSGraphPersonAnnotation alloc] init];
MSGraphItemBody *detail = [[MSGraphItemBody alloc] init];
[detail setContentType: [MSGraphBodyType text]];
[detail setContent:@"I am originally from Australia, but grew up in Moscow, Russia."];
[personAnnotation setDetail:detail];
[personAnnotation setDisplayName:@"About Me"];

NSError *error;
NSData *personAnnotationData = [personAnnotation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAnnotationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```