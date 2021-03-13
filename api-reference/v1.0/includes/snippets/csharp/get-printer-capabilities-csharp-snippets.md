---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2057ec3995ada4ab898842dd99041ae47ced8e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .Select("id,displayName,capabilities")
    .GetAsync();

```