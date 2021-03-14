---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec0b56f09f290d7bf997ff335393ca247deb878e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .GetAsync();

```