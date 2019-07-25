---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8731e1e67bbd684b75b0146f72bd070523b2610a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityPages('D7')
    .Request()
    .GetAsync();

```