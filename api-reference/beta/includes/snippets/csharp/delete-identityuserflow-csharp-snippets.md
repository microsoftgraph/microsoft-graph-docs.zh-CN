---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b079d30b2722b50a97fbab25c91cc606c70d50eb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlows["{id}"]
    .Request()
    .DeleteAsync();

```