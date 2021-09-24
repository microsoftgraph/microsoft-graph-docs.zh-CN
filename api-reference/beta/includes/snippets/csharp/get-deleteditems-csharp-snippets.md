---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c81d77ae76d836df30d5a5b234f2be871ab955ff0d2dda33238dff935b93168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Directory.DeletedItems
    .Request()
    .GetAsync();

```