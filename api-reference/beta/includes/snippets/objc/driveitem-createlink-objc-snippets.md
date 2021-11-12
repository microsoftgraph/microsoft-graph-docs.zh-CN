---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a1f4ef588a272e8eeeecd9ef0b78cf65db3ea90c97402d051bfa32197973f7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220903"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{itemId}/createLink"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *type = @"view";
payloadDictionary[@"type"] = type;

NSString *scope = @"anonymous";
payloadDictionary[@"scope"] = scope;

NSString *password = @"String";
payloadDictionary[@"password"] = password;

NSMutableArray *recipientsList = [[NSMutableArray alloc] init];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipientsList addObject: recipients];
payloadDictionary[@"recipients"] = recipientsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```