---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbce58ba239ff1bf94e5a49c7a41ddf2ad5faa1f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overridesPages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages
    .Request()
    .GetAsync();

```