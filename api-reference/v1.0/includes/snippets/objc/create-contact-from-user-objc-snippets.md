---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90ecb195e0880362725eee185e8dc69d6173b0515e9aa0b0bc23f7b178a49c01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218375"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
[contact setGivenName:@"Pavel"];
[contact setSurname:@"Bansky"];
NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
MSGraphEmailAddress *emailAddresses = [[MSGraphEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@fabrikam.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddressesList addObject: emailAddresses];
[contact setEmailAddresses:emailAddressesList];
NSMutableArray *businessPhonesList = [[NSMutableArray alloc] init];
[businessPhonesList addObject: @"+1 732 555 0102"];
[contact setBusinessPhones:businessPhonesList];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```