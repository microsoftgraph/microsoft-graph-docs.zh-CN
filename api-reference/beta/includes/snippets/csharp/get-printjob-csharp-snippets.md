---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff9bd2e44a02e6dbf7540ca7aed6bce967c81164
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["{id}"].Jobs["{id}"]
    .Request()
    .GetAsync();

```