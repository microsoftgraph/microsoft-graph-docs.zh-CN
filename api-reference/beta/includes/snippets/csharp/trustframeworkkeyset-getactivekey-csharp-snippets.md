---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cbcc57e2a35fe39548236aa293b317e284488c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.KeySets["{id}"]
    .GetActiveKey()
    .Request()
    .GetAsync();

```
