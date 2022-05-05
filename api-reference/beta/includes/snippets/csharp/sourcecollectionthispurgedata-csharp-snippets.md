---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81ac7e6a948cfd615b47edf1dc5d4b75102b2721
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .PurgeData()
    .Request()
    .PostAsync();

```