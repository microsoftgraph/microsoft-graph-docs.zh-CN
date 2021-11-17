---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 944e4dd67950a95c08f53b5ad344f274cc6b64805cc4d4c8a1389268ad178892
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Request()
    .DeleteAsync();

```