---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ad246bd959b4f365bbbb1ea1bab11b0e869e745
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683858"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphPost *post = [[MSGraphPost alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType text]];
[body setContent:@"I attached a reference to a file on OneDrive."];
[post setBody:body];
NSMutableArray *attachmentsList = [[NSMutableArray alloc] init];
MSGraphAttachment *attachments = [[MSGraphAttachment alloc] init];
[attachments setName:@"Personal pictures"];
[attachments setSourceUrl:@"https://contoso.com/personal/mario_contoso_net/Documents/Pics"];
[attachments setProviderType: [MSGraphReferenceAttachmentProvider oneDriveConsumer]];
[attachments setPermission: [MSGraphReferenceAttachmentPermission edit]];
[attachments setIsFolder:@"True"];
[attachmentsList addObject: attachments];
[post setAttachments:attachmentsList];
payloadDictionary[@"post"] = post;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```