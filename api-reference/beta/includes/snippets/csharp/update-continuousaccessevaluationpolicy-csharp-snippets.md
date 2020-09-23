---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc333b4c75fdddedbf6f2fd8160ac7b3e8db6a91
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223139"
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