---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7278a28b88e2c4239fb51edd778fe5ad40fd651
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Emails["{id}"]
    .Request()
    .DeleteAsync();

```