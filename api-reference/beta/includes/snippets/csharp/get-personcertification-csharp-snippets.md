---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00b9755bc1e4962fe97b132a52216f382f2fb258
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = await graphClient.Me.Profile.Certifications["{personCertification-id}"]
    .Request()
    .GetAsync();

```