---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 41e69f88e158f8901c2b5c800447ec0727bf8683
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330407"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookNamedItem *workbookNamedItem = [[MSGraphWorkbookNamedItem alloc] init];
[workbookNamedItem setType:@"type-value"];
[workbookNamedItem setScope:@"scope-value"];
[workbookNamedItem setComment:@"comment-value"];
MSGraphJson *value = [[MSGraphJson alloc] init];
[workbookNamedItem setValue:value];
[workbookNamedItem setVisible: true];

NSError *error;
NSData *workbookNamedItemData = [workbookNamedItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookNamedItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```