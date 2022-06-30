---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd687c990d096492c2c13bcc5bb89cdd0916f2c4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"]
    .Promote()
    .Request()
    .PostAsync();

```