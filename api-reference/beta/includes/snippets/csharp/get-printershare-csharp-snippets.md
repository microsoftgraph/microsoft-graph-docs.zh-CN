---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 874dc68d7587e864f4fca15244a0fdeadb9533e3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.Shares["{id}"]
    .Request()
    .GetAsync();

```