---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7099a81c5b653f7095652bebe6a18096ee47b93e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .ResetToDefault()
    .Request()
    .PostAsync();

```