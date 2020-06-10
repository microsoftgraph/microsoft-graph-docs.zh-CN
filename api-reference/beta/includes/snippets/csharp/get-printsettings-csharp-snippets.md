---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bb87b4569215fc5e56f2487c1086e8e229a6558
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var print = await graphClient.Print
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = print.Settings;

```