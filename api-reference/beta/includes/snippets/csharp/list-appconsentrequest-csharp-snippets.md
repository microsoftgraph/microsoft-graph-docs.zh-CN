---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61f4920f4fa4eddfdaff71efd9baf28d211ba9f67b476873623e71af1471ae43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appConsentRequests = await graphClient.IdentityGovernance.AppConsent.AppConsentRequests
    .Request()
    .GetAsync();

```