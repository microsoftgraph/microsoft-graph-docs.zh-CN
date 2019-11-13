---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c26d655f7c472c8684b4e6c7a64e855982b6065
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Request()
    .DeleteAsync();

```