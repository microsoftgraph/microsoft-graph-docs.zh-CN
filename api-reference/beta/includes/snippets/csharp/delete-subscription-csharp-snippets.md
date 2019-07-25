---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4794d8788d3d40150f96f03065ef5f486232c699
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Subscriptions["{id}"]
    .Request()
    .DeleteAsync();

```