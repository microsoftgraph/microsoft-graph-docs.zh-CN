---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99f5974656937d9a35c2071c5d04ee90b38c3deeeab941b3d4bb7c69ea31edd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.TermStore.Groups["{termStore.group-id}"]
    .Request()
    .GetAsync();

```