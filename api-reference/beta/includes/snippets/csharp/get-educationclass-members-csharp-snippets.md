---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d27a8f94c0f0d28efd03cf14eecca2ac4c1789b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["{educationClass-id}"].Members
    .Request()
    .GetAsync();

```