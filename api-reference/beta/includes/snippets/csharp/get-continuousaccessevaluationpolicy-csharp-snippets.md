---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e4a858b28172919d876b37a3f363972023a1d439711cd480cd154a3c1c70b4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var continuousAccessEvaluationPolicy = await graphClient.Identity.ContinuousAccessEvaluationPolicy
    .Request()
    .GetAsync();

```