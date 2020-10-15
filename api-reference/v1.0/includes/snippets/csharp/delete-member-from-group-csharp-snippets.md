---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e60533aa44b1c658bc73e73ec15774a22a9c39c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Members["{directory-object-id}"].Reference
    .Request()
    .DeleteAsync();

```