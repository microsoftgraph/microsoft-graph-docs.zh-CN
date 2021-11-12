---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f2f41f02406724498b70f659f627be75aad54d19f09ecff92802c3640d8a931
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups["{group-id}"].Reference
    .Request()
    .DeleteAsync();

```