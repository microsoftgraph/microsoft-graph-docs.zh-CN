---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a629f258c7e8e42cebe2711787d56636bcda4ba
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .SetUpResourcesFolder()
    .Request()
    .PostAsync();

```