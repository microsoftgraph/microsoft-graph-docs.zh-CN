---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c8b1b119d1c0fb7ece8678db404cb3cc5f73a8d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.KeySets["{id}"]
    .Request()
    .DeleteAsync();

```