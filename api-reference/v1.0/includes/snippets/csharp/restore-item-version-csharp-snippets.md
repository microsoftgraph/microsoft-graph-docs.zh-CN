---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6a07e1ecc07352b9f70d95d15758deb40ed1ee63
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{item-id}"].Versions["{version-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```