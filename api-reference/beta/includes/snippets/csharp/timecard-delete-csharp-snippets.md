---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b6cb06deb02e7943f1066b3755b3a5b02d2db2b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Request()
    .DeleteAsync();

```