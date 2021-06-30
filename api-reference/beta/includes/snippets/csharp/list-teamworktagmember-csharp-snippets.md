---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 335968be613d4aaf6a982c051a7077fcf1df28b0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members
    .Request()
    .GetAsync();

```