---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb1d8ef71d6b0cfae7d3f911e042f807b2aeceff
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="]
    .Request()
    .Filter("id eq 'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')")
    .Expand("extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')")
    .GetAsync();

```