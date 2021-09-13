---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cea850b672005a04de6641406e565d843591b317bcdf2796dc7f992f24f0b09a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var workingHours = me.MailboxSettings.WorkingHours;

```