---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a07e1ecc07352b9f70d95d15758deb40ed1ee63
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{item-id}"].Versions["{version-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```