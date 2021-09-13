---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd20ead3227de1547c602609e79b40eaccd78afefd51da1db3d287570726ff59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Follow()
    .Request()
    .PostAsync();

```