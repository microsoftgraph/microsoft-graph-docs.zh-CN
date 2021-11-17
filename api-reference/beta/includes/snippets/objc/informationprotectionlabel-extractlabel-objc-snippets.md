---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 801bdf06fd10f92244bd04a31afd18db4559766d800b67ee00df18f7ac244705
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220891"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/policy/labels/extractLabel"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"ContosoLOBApp/1.0" forHTTPHeaderField:@"User-Agent"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphContentInfo *contentInfo = [[MSGraphContentInfo alloc] init];
[contentInfo setFormat: [MSGraphContentFormat default]];
[contentInfo setIdentifier: null];
[contentInfo setState: [MSGraphContentState rest]];
NSMutableArray *metadataList = [[NSMutableArray alloc] init];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled"];
[metadata setValue:@"True"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method"];
[metadata setValue:@"Standard"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate"];
[metadata setValue:@"1/1/0001 12:00:00 AM"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId"];
[metadata setValue:@"cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name"];
[metadata setValue:@"Top Secret"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits"];
[metadata setValue:@"0"];
[metadataList addObject: metadata];
MSGraphKeyValuePair *metadata = [[MSGraphKeyValuePair alloc] init];
[metadata setName:@"MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"];
[metadata setValue:@"00000000-0000-0000-0000-000000000000"];
[metadataList addObject: metadata];
[contentInfo setMetadata:metadataList];
payloadDictionary[@"contentInfo"] = contentInfo;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```