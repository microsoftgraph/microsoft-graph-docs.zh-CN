---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08da636411c59f02b0db9130f2b6f7d9e04d8e8e905f17f7b1c3204e99a34646
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329035"
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