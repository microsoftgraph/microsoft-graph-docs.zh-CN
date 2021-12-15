---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 429650ee8bf9e8fc3dc5e4e72cddf72fc7d83892
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524795"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA *aAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA = [[MSGraphAAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT--0qFRAqk3TNe0QAAAy35RwAA alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```