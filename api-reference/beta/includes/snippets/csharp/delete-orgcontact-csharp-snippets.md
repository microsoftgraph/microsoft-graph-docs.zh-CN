---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f93ebfc3c12d0b88fa77b53fe1eeeee2a94a3191
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```