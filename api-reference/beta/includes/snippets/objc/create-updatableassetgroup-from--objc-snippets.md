---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23783266e87e812393f56866a7f6bfd784ff28b449a7d935b8c8cda63c1feb05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279014"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/updatableAssets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWindowsUpdatesUpdatableAsset *updatableAsset = [[MSGraphWindowsUpdatesUpdatableAsset alloc] init];

NSError *error;
NSData *updatableAssetData = [updatableAsset getSerializedDataWithError:&error];
[urlRequest setHTTPBody:updatableAssetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```