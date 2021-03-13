---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f28d8e000ca4dbba4b72782faac6153edb14b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .DeleteAsync();

```