---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e60533aa44b1c658bc73e73ec15774a22a9c39c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48375740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Members["{directory-object-id}"].Reference
    .Request()
    .DeleteAsync();

```