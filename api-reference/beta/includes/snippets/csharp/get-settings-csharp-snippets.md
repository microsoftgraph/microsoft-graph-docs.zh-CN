---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebfd9bcac4f8f88c33ee9c24fe1c5c8081cde83c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var analytics = await graphClient.Me.Analytics
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = analytics.Settings;

```