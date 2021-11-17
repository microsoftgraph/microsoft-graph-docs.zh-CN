---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 422be43951c3c8ece23605ac5b9bd7ff2b72cdfdd37be87eb9588b629e250a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkHostedContent = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].ColorIcon.HostedContent
    .Request()
    .GetAsync();

```