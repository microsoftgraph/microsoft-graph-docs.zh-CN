---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9be556498cbd47ec4772894ca447af4e0830b7064b5cbe2f96ef734e6cfd246
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = await graphClient.Security.SecureScoreControlProfiles["{secureScoreControlProfile-id}"]
    .Request()
    .GetAsync();

```