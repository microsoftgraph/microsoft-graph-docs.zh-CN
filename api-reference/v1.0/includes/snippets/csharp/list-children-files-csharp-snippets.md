---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad8c97f2020479870d0e89ac222520e698691d24353272d8295c3d5524f7ee0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Children
    .Request()
    .GetAsync();

```