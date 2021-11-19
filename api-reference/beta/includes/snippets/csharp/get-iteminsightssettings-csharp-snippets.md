---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b8d503fb080f553439e031617048eb9dcb5c8a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098343"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var insightsSettings = await graphClient.Organization["{organization-id}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```