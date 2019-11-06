---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d07cd01d0a205e518329ab2e07584d3b2754cce
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Positions["{id}"]
    .Request()
    .DeleteAsync();

```