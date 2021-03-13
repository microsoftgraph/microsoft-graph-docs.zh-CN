---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18f3aeab312e589ab563b1a7f25bbe6ce6659909
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Groups["{group-id}"].Members
    .Request()
    .GetAsync();

```