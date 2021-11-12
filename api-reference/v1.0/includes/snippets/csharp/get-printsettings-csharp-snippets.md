---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 603be6a3addc69123cd1b38a04875fb99ca3659a22bcf7006158ad4643bdeade
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var print = await graphClient.Print
    .Request()
    .Select("Settings")
    .GetAsync();

var settings = print.Settings;

```