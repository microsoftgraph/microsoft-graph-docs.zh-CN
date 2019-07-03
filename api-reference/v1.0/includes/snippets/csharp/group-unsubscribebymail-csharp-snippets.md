---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f05a61da2e621dd6518bb7032f4e146719d5d71
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509265"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .UnsubscribeByMail()
    .Request()
    .PostAsync();

```