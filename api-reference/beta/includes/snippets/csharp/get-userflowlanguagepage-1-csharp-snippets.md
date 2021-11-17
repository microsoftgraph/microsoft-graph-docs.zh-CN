---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f06009fba454e7f2e98d21a3de5d43a194f1b2a96cfa6a5f3aa4a5778123fb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var defaultPages = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].DefaultPages
    .Request()
    .GetAsync();

```