---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5914c8e8011f9108d0e1a64eb371cd4f1a973de7db0f833e41833e5c004d58c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105009"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
MSGraphPhysicalAddress *homeAddress = [[MSGraphPhysicalAddress alloc] init];
[homeAddress setStreet:@"123 Some street"];
[homeAddress setCity:@"Seattle"];
[homeAddress setState:@"WA"];
[homeAddress setPostalCode:@"98121"];
[contact setHomeAddress:homeAddress];
[contact setBirthday:@"1974-07-22"];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```