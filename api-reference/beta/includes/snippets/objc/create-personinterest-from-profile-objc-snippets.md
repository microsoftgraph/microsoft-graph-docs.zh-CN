---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea58480da337ce0058561377b2dda023802cf0fa694116bfd58c669df49ed149
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279589"
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