---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fef10eb98468558b7b6e1b43d22e2bafbdf4aee5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["{group-id}"].Events
    .Request()
    .GetAsync();

```