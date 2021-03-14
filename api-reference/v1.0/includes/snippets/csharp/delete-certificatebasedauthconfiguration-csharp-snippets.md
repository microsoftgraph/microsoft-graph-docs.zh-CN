---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 658cce317d69187fcb913c0a960a80ec3b871af3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration["{certificateBasedAuthConfiguration-id}"]
    .Request()
    .DeleteAsync();

```