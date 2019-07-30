---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f6e7255dc7e91a0f0d8f0e6ee5feb3efb28472c9
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participant = await graphClient.App.Calls["{id}"].Participants["{id}"]
    .Request()
    .GetAsync();

```