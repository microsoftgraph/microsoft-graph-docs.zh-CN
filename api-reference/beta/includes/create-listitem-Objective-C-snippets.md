---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0e201abb16c2b68be6cb61242d16a3b59c21ac4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318229"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items/{item-id}/fields"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFieldValueSet *fieldValueSet = [[MSGraphFieldValueSet alloc] init];
[fieldValueSet setColor:@"Fuchsia"];
[fieldValueSet setQuantity: 934];

NSError *error;
NSData *fieldValueSetData = [fieldValueSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:fieldValueSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```