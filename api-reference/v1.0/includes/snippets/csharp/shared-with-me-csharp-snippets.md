---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e845e305eb7f10adb4b737b04bd5c6660f0dc84
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive.SharedWithMe()
    .Request()
    .GetAsync();

```