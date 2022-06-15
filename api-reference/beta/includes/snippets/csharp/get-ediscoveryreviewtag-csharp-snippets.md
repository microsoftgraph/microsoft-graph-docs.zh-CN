---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cd6a0a78b5c0634cbdd1264807355788c077006
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryReviewTag = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Tags["{security.ediscoveryReviewTag-id}"]
    .Request()
    .GetAsync();

```