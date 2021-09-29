---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac5b8fa08eb1f69e41aa2c2e9e9a08b7843b068
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var localizations = await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .GetAsync();

```