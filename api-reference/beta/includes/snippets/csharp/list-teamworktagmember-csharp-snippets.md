---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd30bba6a7a21f30028f7ffd577bb00851ce33e7cd0f3c2f6f58eefa62ab6e37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members
    .Request()
    .GetAsync();

```