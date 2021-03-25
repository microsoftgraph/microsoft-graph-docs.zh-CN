---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55cece7bdea29ba88c0a3c663bb8b4a42c0359e0
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var adminConsentRequestPolicy = await graphClient.Policies.AdminConsentRequestPolicy
    .Request()
    .GetAsync();

```