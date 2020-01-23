---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c45148fb0b3868f12913187bba95dcb2ad14b86
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies["claimsMappingPolicies"].{id}
    .Request()
    .DeleteAsync();

```