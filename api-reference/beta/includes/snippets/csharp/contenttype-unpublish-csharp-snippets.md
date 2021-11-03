---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c4dbdac6e878a2b1cf17044b753ae649c0574b2444ea6df05695ed28bba5f5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Unpublish()
    .Request()
    .PostAsync();

```