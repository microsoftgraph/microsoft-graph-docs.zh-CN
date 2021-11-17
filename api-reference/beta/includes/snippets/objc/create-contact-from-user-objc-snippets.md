---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 619d3135797140dc7ab118898bbfe757957fe223b1d7f5ed31d6ca9ecde01aa3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104661"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/contacts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContact *contact = [[MSGraphContact alloc] init];
[contact setGivenName:@"Pavel"];
[contact setSurname:@"Bansky"];
NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@contoso.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setType: [MSGraphEmailType personal]];
[emailAddressesList addObject: emailAddresses];
MSGraphTypedEmailAddress *emailAddresses = [[MSGraphTypedEmailAddress alloc] init];
[emailAddresses setAddress:@"pavelb@fabrikam.onmicrosoft.com"];
[emailAddresses setName:@"Pavel Bansky"];
[emailAddresses setType: [MSGraphEmailType other]];
[emailAddresses setOtherLabel:@"Volunteer work"];
[emailAddressesList addObject: emailAddresses];
[contact setEmailAddresses:emailAddressesList];
NSMutableArray *phonesList = [[NSMutableArray alloc] init];
MSGraphPhone *phones = [[MSGraphPhone alloc] init];
[phones setNumber:@"+1 732 555 0102"];
[phones setType: [MSGraphPhoneType business]];
[phonesList addObject: phones];
[contact setPhones:phonesList];

NSError *error;
NSData *contactData = [contact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```