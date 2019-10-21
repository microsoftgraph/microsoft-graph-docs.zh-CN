---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 250eeb29f921ca05f0a21c8e1af944dcb18790a5
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35707508"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts/AAMkADh6v5AAAvgTCEAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setType: [MSGraphEmailType personal]];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setAddress:@"pavelb@adatum.onmicrosoft.com"];
[emailAddressesList addObject: emailAddresses];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@fabrikam.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setType: [MSGraphEmailType other]];
[emailAddresses setOtherLabel:@"Volunteer work"];
[emailAddressesList addObject: emailAddresses];
[contact setEmailAddresses:emailAddressesList];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```