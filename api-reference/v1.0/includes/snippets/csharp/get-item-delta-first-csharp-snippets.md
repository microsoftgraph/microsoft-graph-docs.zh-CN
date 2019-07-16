---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 72a55c21f4a58e4a1affc4bfcec6f8faa01f0287
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root.Delta()
    .Request()
    .GetAsync();

```