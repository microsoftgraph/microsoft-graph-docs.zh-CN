---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19a31bd49fcc9dc96a215f6e0c45a6a0f533786f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Unsubmit()
    .Request()
    .PostAsync();

```