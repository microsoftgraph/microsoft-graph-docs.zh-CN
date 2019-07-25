---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17a68e67ac476b5bf226dbf85dc640148de8f1fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["{id}"].InstalledApps
    .Request()
    .GetAsync();

```