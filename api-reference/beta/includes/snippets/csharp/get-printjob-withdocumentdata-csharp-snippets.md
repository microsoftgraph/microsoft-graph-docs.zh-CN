---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a151aa4debd4ed57d567d0ed7651d7b813d26d6200d92efa41ae5fb43b27d606
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Request()
    .Expand("documents")
    .GetAsync();

```