---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0c4a7e8a78750893e9d90d5924a57dc8ae699bb9302353fa8fdf1f8913821ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = await graphClient.Me.Profile.Projects["{projectParticipation-id}"]
    .Request()
    .GetAsync();

```