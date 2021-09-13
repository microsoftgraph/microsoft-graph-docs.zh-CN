---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66080f0a23f2bd5f23962068d03f487cb4f0371da148ba9dabdcad7261602315
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903209"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreementAcceptances = await graphClient.Me.AgreementAcceptances
    .Request()
    .GetAsync();

```