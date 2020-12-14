---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9711b78ea4109d6d564f935aa924277f684b892
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Users["66825e03-7ef5-42da-9069-724602c31f6b"].Presence
    .Request()
    .GetAsync();

```