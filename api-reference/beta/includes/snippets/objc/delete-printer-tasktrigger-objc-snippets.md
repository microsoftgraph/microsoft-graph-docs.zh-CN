---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb02014eaa944f3d799184b0df2b17bb1653f8612a9996879af0638d89434747
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105546"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec"]]];
[urlRequest setHTTPMethod:@"DELETE"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```