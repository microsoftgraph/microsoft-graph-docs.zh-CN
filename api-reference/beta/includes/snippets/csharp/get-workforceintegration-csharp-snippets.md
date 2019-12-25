---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7274f06fcd816db0da48be70cf6fa6a46bb63d86
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = await graphClient.Teamwork.WorkforceIntegrations["{workforceintegrationid}"]
    .Request()
    .GetAsync();

```