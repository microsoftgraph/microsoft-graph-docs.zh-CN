---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5c66f747c8b69d3d83061835f55ab05299070b8831a9010009677908a731409
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"]
    .Request()
    .DeleteAsync();

```