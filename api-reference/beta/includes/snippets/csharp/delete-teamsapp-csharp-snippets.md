---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83f2f48b9ea144594c7a501cab57d3ef793f9392
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppCatalogs.TeamsApps["06805b9e-77e3-4b93-ac81-525eb87513b8"]
    .Request()
    .DeleteAsync();

```