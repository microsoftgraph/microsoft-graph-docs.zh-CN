---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c018f85fd484f2488ec30316884736d5d150065078d05c12b992fc87712b5af1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealth = await graphClient.Admin.ServiceAnnouncement.HealthOverviews["{serviceHealth-id}"]
    .Request()
    .Expand("issues")
    .GetAsync();

```