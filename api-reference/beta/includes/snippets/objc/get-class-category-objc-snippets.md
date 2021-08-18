---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c32fb18f84ed9c8ffd7d0a64f9fe3a91a2474abfb9d5bf86831db9a8ceda037d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163146"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEducationCategory *educationCategory = [[MSGraphEducationCategory alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```