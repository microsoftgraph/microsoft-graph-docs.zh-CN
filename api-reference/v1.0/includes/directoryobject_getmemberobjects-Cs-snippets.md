---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 939dafdfa2983ee68ebb771a3b75a8d3bb465a08
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{object-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```