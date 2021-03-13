---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52a5da2eae3b28401a30e2b0df350969891b1588
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781669"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var controls = await graphClient.Programs["{program-id}"].Controls
    .Request()
    .GetAsync();

```