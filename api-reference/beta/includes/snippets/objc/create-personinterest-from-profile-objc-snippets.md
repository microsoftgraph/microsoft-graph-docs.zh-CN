---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5691c9e20a66a4b6a768aeee1d9dd53814f9d1ae
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821193"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/interests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonInterest *personInterest = [[MSGraphPersonInterest alloc] init];
NSMutableArray *categoriesList = [[NSMutableArray alloc] init];
[categoriesList addObject: @"Sports"];
[personInterest setCategories:categoriesList];
[personInterest setDescription:@"World's greatest football club"];
[personInterest setDisplayName:@"Chelsea FC"];
[personInterest setWebUrl:@"https://www.chelseafc.com"];

NSError *error;
NSData *personInterestData = [personInterest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personInterestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```