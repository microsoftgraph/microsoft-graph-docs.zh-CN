---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6915885ea09e89b122968b4589be65065c3c778
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{notebook-id}"]
    .Request()
    .GetAsync();

```