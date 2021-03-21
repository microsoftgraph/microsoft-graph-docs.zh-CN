---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc57f5524b85e866518670ecf6a8db2fc6d28bee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].DefaultPages["{userFlowLanguagePage-id}"].Content
    .Request()
    .GetAsync();

```