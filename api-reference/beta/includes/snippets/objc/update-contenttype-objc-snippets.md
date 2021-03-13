---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44e79968012014274938dd9c9ca7914948d6378e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773303"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/contentTypes/{contentType-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContentType *contentType = [[MSGraphContentType alloc] init];
[contentType setName:@"updatedCt"];
MSGraphDocumentSet *documentSet = [[MSGraphDocumentSet alloc] init];
[documentSet setShouldPrefixNameToFile: true];
NSMutableArray *allowedContentTypesList = [[NSMutableArray alloc] init];
MSGraphContentTypeInfo *allowedContentTypes = [[MSGraphContentTypeInfo alloc] init];
[allowedContentTypes setId:@"0x0101"];
[allowedContentTypes setName:@"Document"];
[allowedContentTypesList addObject: allowedContentTypes];
[documentSet setAllowedContentTypes:allowedContentTypesList];
NSMutableArray *defaultContentsList = [[NSMutableArray alloc] init];
MSGraphDocumentSetContent *defaultContents = [[MSGraphDocumentSetContent alloc] init];
[defaultContents setFileName:@"a.txt"];
MSGraphDocumentSetContent *contentType = [[MSGraphDocumentSetContent alloc] init];
[contentType setId:@"0x0101"];
[defaultContents setContentType:contentType];
[defaultContentsList addObject: defaultContents];
MSGraphDocumentSetContent *defaultContents = [[MSGraphDocumentSetContent alloc] init];
[defaultContents setFileName:@"b.txt"];
MSGraphDocumentSetContent *contentType = [[MSGraphDocumentSetContent alloc] init];
[contentType setId:@"0x0101"];
[defaultContents setContentType:contentType];
[defaultContentsList addObject: defaultContents];
[documentSet setDefaultContents:defaultContentsList];
NSMutableArray *sharedColumnsList = [[NSMutableArray alloc] init];
MSGraphColumnDefinition *sharedColumns = [[MSGraphColumnDefinition alloc] init];
[sharedColumns setName:@"Description"];
[sharedColumns setId:@"cbb92da4-fd46-4c7d-af6c-3128c2a5576e"];
[sharedColumnsList addObject: sharedColumns];
MSGraphColumnDefinition *sharedColumns = [[MSGraphColumnDefinition alloc] init];
[sharedColumns setName:@"Address"];
[sharedColumns setId:@"fc2e188e-ba91-48c9-9dd3-16431afddd50"];
[sharedColumnsList addObject: sharedColumns];
[documentSet setSharedColumns:sharedColumnsList];
NSMutableArray *welcomePageColumnsList = [[NSMutableArray alloc] init];
MSGraphColumnDefinition *welcomePageColumns = [[MSGraphColumnDefinition alloc] init];
[welcomePageColumns setName:@"Address"];
[welcomePageColumns setId:@"fc2e188e-ba91-48c9-9dd3-16431afddd50"];
[welcomePageColumnsList addObject: welcomePageColumns];
[documentSet setWelcomePageColumns:welcomePageColumnsList];
[contentType setDocumentSet:documentSet];

NSError *error;
NSData *contentTypeData = [contentType getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contentTypeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```