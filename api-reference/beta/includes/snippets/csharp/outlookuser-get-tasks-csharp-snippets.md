---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 972cf76b767313a7d745156f8b301c6f277a1b402fcf3c3df1f2fdefc317965d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Outlook.Tasks
    .Request()
    .GetAsync();

```