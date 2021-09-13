---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 536b9a711c3337f482c5c3e1affb772dbf39302f70c5564ca428090936af850a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332549"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOrganization *organization = [[MSGraphOrganization alloc] init];
NSMutableArray *marketingNotificationEmailsList = [[NSMutableArray alloc] init];
[marketingNotificationEmailsList addObject: @"marketing@contoso.com"];
[organization setMarketingNotificationEmails:marketingNotificationEmailsList];
MSGraphPrivacyProfile *privacyProfile = [[MSGraphPrivacyProfile alloc] init];
[privacyProfile setContactEmail:@"alice@contoso.com"];
[privacyProfile setStatementUrl:@"https://contoso.com/privacyStatement"];
[organization setPrivacyProfile:privacyProfile];
NSMutableArray *securityComplianceNotificationMailsList = [[NSMutableArray alloc] init];
[securityComplianceNotificationMailsList addObject: @"security@contoso.com"];
[organization setSecurityComplianceNotificationMails:securityComplianceNotificationMailsList];
NSMutableArray *securityComplianceNotificationPhonesList = [[NSMutableArray alloc] init];
[securityComplianceNotificationPhonesList addObject: @"(123) 456-7890"];
[organization setSecurityComplianceNotificationPhones:securityComplianceNotificationPhonesList];
NSMutableArray *technicalNotificationMailsList = [[NSMutableArray alloc] init];
[technicalNotificationMailsList addObject: @"tech@contoso.com"];
[organization setTechnicalNotificationMails:technicalNotificationMailsList];

NSError *error;
NSData *organizationData = [organization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:organizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```