---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 933bdc93a68e12d17612ae35b86a8f6e0fa6982d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```