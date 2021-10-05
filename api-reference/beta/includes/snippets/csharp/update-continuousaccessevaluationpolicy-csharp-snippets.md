---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df7703d1015229965a1462f7dd0c3c81ae482738cd925f3b48061f013f1cb2eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328932"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var continuousAccessEvaluationPolicy = new ContinuousAccessEvaluationPolicy
{
    Users = new List<String>()
    {
        "88139f01-1f8d-4c06-ad74-a2544cee9aee"
    },
    Groups = new List<String>()
    {
        "9972fb3f-7a40-49f5-85f6-129d9dfbd47a",
        "ea178055-4713-4d9a-a06c-ff17466b7e77"
    }
};

await graphClient.Identity.ContinuousAccessEvaluationPolicy
    .Request()
    .UpdateAsync(continuousAccessEvaluationPolicy);

```