---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea2e61a58ae4a673cbe310eb6ee9dfd1201e003a9efbd4c4dc3eea681367ac30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Versions["{driveItemVersion-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```