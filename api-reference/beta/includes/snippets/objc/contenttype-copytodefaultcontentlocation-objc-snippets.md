---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64a757112a5cb36564c3d960925929aa16664712
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771090"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphItemReference *sourceFile = [[MSGraphItemReference alloc] init];
MSGraphSharepointIds *sharepointIds = [[MSGraphSharepointIds alloc] init];
[sharepointIds setListId:@"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0"];
[sharepointIds setListItemId:@"2"];
[sourceFile setSharepointIds:sharepointIds];
payloadDictionary[@"sourceFile"] = sourceFile;

NSString *destinationFileName = @"newname.txt";
payloadDictionary[@"destinationFileName"] = destinationFileName;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```