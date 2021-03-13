---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bb87b4569215fc5e56f2487c1086e8e229a6558
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777255"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var print = await graphClient.Print
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = print.Settings;

```