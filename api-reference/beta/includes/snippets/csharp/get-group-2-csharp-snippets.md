---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d7bdd3e22d02d6b2780627e4fc6b95c7f79e07b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.TermStore.Groups
    .Request()
    .GetAsync();

```