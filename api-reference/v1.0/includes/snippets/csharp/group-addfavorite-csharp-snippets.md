---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f39562c0802d38e5ff186b63e6a3fa4f6162ff7f16875ecbe0d40269f710f26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .AddFavorite()
    .Request()
    .PostAsync();

```