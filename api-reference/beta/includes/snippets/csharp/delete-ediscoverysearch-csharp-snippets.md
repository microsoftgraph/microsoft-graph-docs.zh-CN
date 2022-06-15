---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2beb626a1e55a2f02252f8b0b0aab077a28af6e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094747"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"]
    .Request()
    .DeleteAsync();

```