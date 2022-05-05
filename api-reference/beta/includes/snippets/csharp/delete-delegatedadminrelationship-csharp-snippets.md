---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4b3b72af5678f8b87bad47b9b2d3795c32f7746
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"]
    .Request()
    .Header("If-Match","W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"")
    .DeleteAsync();

```