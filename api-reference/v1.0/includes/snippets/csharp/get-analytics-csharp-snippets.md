---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 815ccc127a2eb75e63a32083bfb737dc290009f41bd3727f0efcd0ecfa3455e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903890"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAnalytics = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Analytics
    .Request()
    .GetAsync();

```