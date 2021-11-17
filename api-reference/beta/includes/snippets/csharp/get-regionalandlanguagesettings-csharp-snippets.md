---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44ef226b33e78a7d76142f25edf34df914877be07df807ca79f1eb9846629de1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var regionalAndLanguageSettings = await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .GetAsync();

```