---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bc7fe994318addc4ca1e973bd03fe18d971909f740b7acb7bbe5fcb5ac7e58d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .ReprocessLicenseAssignment()
    .Request()
    .PostAsync();

```