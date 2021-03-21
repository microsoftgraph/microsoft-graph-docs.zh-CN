---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fa357e93568c75ae52df08d4abc3c383caaa4d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var defaultPages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].DefaultPages
    .Request()
    .GetAsync();

```