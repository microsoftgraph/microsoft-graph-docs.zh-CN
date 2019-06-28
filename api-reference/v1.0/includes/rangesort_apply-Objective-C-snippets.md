---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cded3f4273958c4c2d2880cfa74f005e7ae361e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323190"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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