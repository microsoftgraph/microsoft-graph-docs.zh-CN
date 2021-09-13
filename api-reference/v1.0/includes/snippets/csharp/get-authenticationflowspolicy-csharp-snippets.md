---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e72b301ef41e9348a481410e0f117273f5303a1731047a7a37822f1bd900819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationFlowsPolicy = await graphClient.Policies.AuthenticationFlowsPolicy
    .Request()
    .GetAsync();

```