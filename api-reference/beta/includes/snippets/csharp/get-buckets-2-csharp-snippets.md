---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 707831aa31286305e45a7bdcc7f859fd92a08e7198b279c32803edb93130a37b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["{plannerPlan-id}"].Buckets
    .Request()
    .GetAsync();

```