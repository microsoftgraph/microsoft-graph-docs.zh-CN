---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec0b56f09f290d7bf997ff335393ca247deb878e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .GetAsync();

```