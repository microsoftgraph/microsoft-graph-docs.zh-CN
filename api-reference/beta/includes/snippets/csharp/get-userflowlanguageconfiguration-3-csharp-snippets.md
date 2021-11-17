---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef756f25fdcb52400a6065d53e77d1de43d330319ad48c80acf407b203c1aed8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowLanguageConfiguration = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"]
    .Request()
    .GetAsync();

```