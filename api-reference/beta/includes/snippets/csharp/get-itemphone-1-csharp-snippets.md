---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d40ffd38d9f70f2ce1a4297937143c287831edba435f68dd372f27aeafd9d5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = await graphClient.Me.Profile.Phones["{itemPhone-id}"]
    .Request()
    .GetAsync();

```