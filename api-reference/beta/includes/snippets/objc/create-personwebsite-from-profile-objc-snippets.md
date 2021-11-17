---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b47376d55eb18d875c4e9d59e4817f2af24d170beabc237a745551a82d54dc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273844"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/websites"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonWebsite *personWebsite = [[MSGraphPersonWebsite alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"football"];
[personWebsite setCategories:categoriesList];
[personWebsite setDisplayName:@"Lyn Damer"];
[personWebsite setWebUrl:@"www.lyndamer.no"];

NSError *error;
NSData *personWebsiteData = [personWebsite getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personWebsiteData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```