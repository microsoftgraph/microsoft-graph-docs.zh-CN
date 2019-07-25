---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3f9106ae49c978a97382349a069244a78ae994e6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"]
    .Request()
    .DeleteAsync();

```