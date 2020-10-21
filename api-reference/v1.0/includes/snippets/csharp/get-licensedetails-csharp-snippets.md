---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25c3f9dd496c2a2bb6eee627a0d0b5b8b9788ca0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var licenseDetails = await graphClient.Me.LicenseDetails
    .Request()
    .GetAsync();

```