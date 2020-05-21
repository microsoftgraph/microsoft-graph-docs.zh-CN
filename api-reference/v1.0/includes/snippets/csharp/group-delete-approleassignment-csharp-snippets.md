---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d2c9ada97052081f8e38f96c91c162a885e05e4
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].AppRoleAssignments["{id}"]
    .Request()
    .DeleteAsync();

```