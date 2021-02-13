---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f9c00176b519d672e7790ff611d2568a98a95cb
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{sitesId}"].Permissions["{permissionId}"]
    .Request()
    .DeleteAsync();

```