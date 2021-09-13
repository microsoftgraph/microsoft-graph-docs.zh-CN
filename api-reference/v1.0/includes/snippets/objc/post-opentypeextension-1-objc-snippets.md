---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3a205639447881946e20ef6223cde6b92e26170e97b12ec87891ded513cbbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220006"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"Annual review"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"You should be proud!"];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"rufus@contoso.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];
NSMutableArray *extensionsList = [[NSMutableArray alloc] init];
MSGraphExtension *extensions = [[MSGraphExtension alloc] init];
[extensions setExtensionName:@"Com.Contoso.Referral"];
[extensions setCompanyName:@"Wingtip Toys"];
[extensions setExpirationDate: "2015-12-30T11:00:00Z"];
[extensions setDealValue: 10000];
[extensionsList addObject: extensions];
[message setExtensions:extensionsList];

NSError *error;
NSData *messageData = [message getSerializedDataWithError:&error];
[urlRequest setHTTPBody:messageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```