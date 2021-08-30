---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49c9875c4a6df6a6d6aef819c7f9654b8e5f5b264f67bde0cf0f36cd7f62f00d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .GetAsync();

```