---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 869ec00d7e74764be0a7f544d18390afe0b0cd2b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes
    .Delta()
    .Request()
    .GetAsync();

```