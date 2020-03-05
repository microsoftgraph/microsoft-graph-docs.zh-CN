---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 622420f06dd03d73b1a67823609b5458d5c05b1d
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies["tokenLifetimePolicies"].{id}
    .Request()
    .DeleteAsync();

```