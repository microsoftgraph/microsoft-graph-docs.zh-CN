---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cb261939f5f2d2d82008eb4d8dfc264bf3fa19bfcab893ed2e108d2648bcdc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218853"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.AppCatalogs.TeamsApps["{teamsApp-id}"].AppDefinitions["{teamsAppDefinition-id}"].OutlineIcon.HostedContent.Content
    .Request()
    .GetAsync();

```