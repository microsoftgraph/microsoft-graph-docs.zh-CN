---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a0ee6ca321292fe3ce7226aad675549697c27f4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "48223541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var teamsApp = new System.IO.MemoryStream(Encoding.UTF8.GetBytes("[Zip file containing a Teams app package]"));

await graphClient.AppCatalogs.TeamsApps["06805b9e-77e3-4b93-ac81-525eb87513b8"]
    .Request()
    .PutAsync(teamsApp);

```