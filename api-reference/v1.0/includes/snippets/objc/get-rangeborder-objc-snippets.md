---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3f617bbed82c34362d721a1af7edc4274a556b24e93dff7dc4bb1e3c628d7f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218377"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWorkbookRangeBorder *workbookRangeBorder = [[MSGraphWorkbookRangeBorder alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```