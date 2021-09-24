---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70dd4976f8e47acd2021e536c81f7e4feeff6cae
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507590"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/claimsMappingPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphClaimsMappingPolicy *claimsMappingPolicy = [[MSGraphClaimsMappingPolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"{"ClaimsMappingPolicy":{"Version":1,"IncludeBasicClaimSet":"true","ClaimsSchema": [{"Source":"user","ID":"userprincipalname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier"},{"Source":"user","ID":"givenname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname"},{"Source":"user","ID":"displayname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/name"},{"Source":"user","ID":"surname","SamlClaimType":"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname"},{"Source":"user","ID":"userprincipalname","SamlClaimType":"username"}],"ClaimsTransformation":[{"ID":"CreateTermsOfService","TransformationMethod":"CreateStringClaim","InputParameters": [{"ID":"value","DataType":"string", "Value":"sandbox"}],"OutputClaims":[{"ClaimTypeReferenceId":"TOS","TransformationClaimType":"createdClaim"}]}]}}"];
[claimsMappingPolicy setDefinition:definitionList];
[claimsMappingPolicy setDisplayName:@"Test1234"];

NSError *error;
NSData *claimsMappingPolicyData = [claimsMappingPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:claimsMappingPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```