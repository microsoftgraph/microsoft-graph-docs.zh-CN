---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3ffe15098467882176bd73fc67f213cad18546f0dbbc5f8de1b44cc97e84cd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"]
    .Request()
    .GetAsync();

```