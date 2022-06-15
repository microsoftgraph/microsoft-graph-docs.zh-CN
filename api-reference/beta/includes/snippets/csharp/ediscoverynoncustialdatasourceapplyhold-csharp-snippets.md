---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ceb05e6a4bef7861cc1aebac113e64576ef8ff4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].NoncustodialDataSources["{security.ediscoveryNoncustodialDataSource-id}"]
    .ApplyHold()
    .Request()
    .PostAsync();

```