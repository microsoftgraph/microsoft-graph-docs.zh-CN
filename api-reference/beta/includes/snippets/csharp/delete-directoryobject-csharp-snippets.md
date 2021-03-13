---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c9719e720a88616cfd0ea2986c0512ce107a688
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .DeleteAsync();

```