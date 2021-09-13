---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2259ef63dd61514fd5c933c4603f54244c301d68b52e5b064e6b8eeb9eecb5ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219934"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/publications"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPublication *itemPublication = [[MSGraphItemPublication alloc] init];
[itemPublication setDescription:@"One persons journey to the top of the branding management field."];
[itemPublication setDisplayName:@"Got Brands? The story of Innocenty Popov and his journey to the top."];
[itemPublication setPublishedDate:@"Date"];
[itemPublication setPublisher:@"International Association of Branding Management Publishing"];
[itemPublication setThumbnailUrl:@"https://iabm.io/sdhdfhsdhshsd.jpg"];
[itemPublication setWebUrl:@"https://www.iabm.io"];

NSError *error;
NSData *itemPublicationData = [itemPublication getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPublicationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```