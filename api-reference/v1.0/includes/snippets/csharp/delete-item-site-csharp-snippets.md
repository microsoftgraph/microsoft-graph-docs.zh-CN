---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 649f50e9533e06bb5499e36232e036f7aedec1a0da662841860f5794ea5b2b4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .Request()
    .DeleteAsync();

```