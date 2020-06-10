---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4e221bbfed74de1604bed1498e2c0f768299252
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Me.Events
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview")
    .GetAsync();

```