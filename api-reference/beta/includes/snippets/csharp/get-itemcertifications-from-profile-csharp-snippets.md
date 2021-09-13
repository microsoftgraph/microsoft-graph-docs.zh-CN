---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aedeee472ea5f09a128a5bf25ebba0991cc14002fb8335471c0a7c8a03a5a8f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218994"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certifications = await graphClient.Me.Profile.Certifications
    .Request()
    .GetAsync();

```