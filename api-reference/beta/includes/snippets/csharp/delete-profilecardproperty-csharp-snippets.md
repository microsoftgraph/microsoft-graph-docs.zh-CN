---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fdc67007cd2f70bc1328044f7e2e80c119b339aa05234df03cbbdc73f002634
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties["{profileCardProperty-id}"]
    .Request()
    .DeleteAsync();

```