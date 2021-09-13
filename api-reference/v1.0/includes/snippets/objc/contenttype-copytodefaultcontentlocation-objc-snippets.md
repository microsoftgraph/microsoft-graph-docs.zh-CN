---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fde4ac40ecce5a88fb76ddd7bde3e24c4581cba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147631"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation"]]];
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