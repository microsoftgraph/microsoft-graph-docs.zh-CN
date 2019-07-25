---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84418c60369e382d63841b4affdc0b4d6aacfc7c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].AcceptedSenders.References
    .Request()
    .DeleteAsync();

```