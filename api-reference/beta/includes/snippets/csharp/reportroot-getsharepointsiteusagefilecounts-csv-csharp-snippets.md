---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c387ce030dbacc9eb12ea69196639ab2a36f74c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageFileCounts = await graphClient.Reports.GetSharePointSiteUsageFileCounts('D7')
    .Request()
    .GetAsync();

```