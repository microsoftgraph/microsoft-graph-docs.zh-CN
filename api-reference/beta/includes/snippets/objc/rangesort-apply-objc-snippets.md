---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cd8728a786645a5d6ff42ba88d44a259473b685ff7ddde99debb495b09c378b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333440"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{id}/workbook/names/{name}/range/sort/apply"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *fieldsList = [[NSMutableArray alloc] init];
MSGraphWorkbookSortField *fields = [[MSGraphWorkbookSortField alloc] init];
[fields setKey: 99];
[fields setSortOn:@"sortOn-value"];
[fields setAscending: true];
[fields setColor:@"color-value"];
[fields setDataOption:@"dataOption-value"];
MSGraphWorkbookIcon *icon = [[MSGraphWorkbookIcon alloc] init];
[icon setSet:@"set-value"];
[icon setIndex: 99];
[fields setIcon:icon];
[fieldsList addObject: fields];
payloadDictionary[@"fields"] = fieldsList;

BOOL matchCase = YES;
payloadDictionary[@"matchCase"] = matchCase;

BOOL hasHeaders = YES;
payloadDictionary[@"hasHeaders"] = hasHeaders;

NSString *orientation = @"orientation-value";
payloadDictionary[@"orientation"] = orientation;

NSString *method = @"method-value";
payloadDictionary[@"method"] = method;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```