---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a05d718d7da4d5c72caa0aa71c82c17e3e89b36
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Schools
    .Delta()
    .Request()
    .GetAsync();

```