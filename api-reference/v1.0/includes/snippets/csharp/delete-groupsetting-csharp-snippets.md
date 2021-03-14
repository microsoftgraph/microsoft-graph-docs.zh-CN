---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f0a74f24901b454e6f15c25cba69f911b58efb5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .DeleteAsync();

```