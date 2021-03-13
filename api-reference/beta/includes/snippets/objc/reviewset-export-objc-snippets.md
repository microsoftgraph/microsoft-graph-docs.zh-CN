---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f038893f6083e453a87d71817b2ad33e84707de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772869"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *outputName = @"2020-12-06 Contoso investigation export";
payloadDictionary[@"outputName"] = outputName;

NSString *description = @"Export for the Contoso investigation";
payloadDictionary[@"description"] = description;

MSGraphEdiscoveryExportOptions *exportOptions = [MSGraphEdiscoveryExportOptions originalFiles];
payloadDictionary[@"exportOptions"] = exportOptions;

MSGraphEdiscoveryExportFileStructure *exportStructure = [MSGraphEdiscoveryExportFileStructure directory];
payloadDictionary[@"exportStructure"] = exportStructure;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```