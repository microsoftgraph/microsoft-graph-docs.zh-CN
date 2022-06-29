---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3356f7263f7cfcbb679213e25f177e67020d1dc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryNoncustodialDataSourceReference = new ReferenceRequestBody
{
    ODataId = "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].NoncustodialSources.References
    .Request()
    .AddAsync(ediscoveryNoncustodialDataSourceReference);

```