---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16962fc165003974925c5d464e4a35818d355cf5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```