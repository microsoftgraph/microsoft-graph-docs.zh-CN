---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4055577197c00f87bd96598183101f34afcb75f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616351"
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