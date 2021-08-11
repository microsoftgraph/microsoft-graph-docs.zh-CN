---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 071a6d9e4891a1ce151047af8cfc9685546c387be6fcb454c8938392ffe55943
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129730"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Calendar.Events["AAMkADJXJGu0AABf02qwAAA="]
    .Request()
    .GetAsync();

```