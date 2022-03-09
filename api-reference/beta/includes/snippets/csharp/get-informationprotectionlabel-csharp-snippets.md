---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba797935c3c9dad04f2ea4a7c474bf5b4a579e9c66da4b0930b52704c64c89de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var informationProtectionLabel = await graphClient.Me.InformationProtection.Policy.Labels["{informationProtectionLabel-id}"]
    .Request()
    .GetAsync();

```