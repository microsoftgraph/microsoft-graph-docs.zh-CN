---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 491ad4b4f40ad9e4ed79bba7dd1565726a19252e
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamsId}"].Members["{membership-id}"]
    .Request()
    .DeleteAsync();

```