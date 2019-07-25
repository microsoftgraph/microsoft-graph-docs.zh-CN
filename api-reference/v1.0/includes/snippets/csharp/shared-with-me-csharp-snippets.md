---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ff5c37301921c418ae9241b1d74ba1d48063d9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive
    .SharedWithMe()
    .Request()
    .GetAsync();

```