---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdd40850409273d2ebb0882fb4cc3c92323c83f1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.Communications.Calls["2f1a1100-b174-40a0-aba7-0b405e01ed92"]
    .Request()
    .GetAsync();

```