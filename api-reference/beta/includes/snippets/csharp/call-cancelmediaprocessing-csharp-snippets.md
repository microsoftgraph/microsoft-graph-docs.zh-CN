---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c9dcd81c8feba021c932b71950c9bbc378807c0
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var all = true;

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .CancelMediaProcessing(clientContext)
    .Request()
    .PostAsync();

```