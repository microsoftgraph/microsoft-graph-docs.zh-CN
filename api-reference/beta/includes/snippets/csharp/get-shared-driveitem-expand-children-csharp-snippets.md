---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22e520eb5fb5b4d5807ac7c83393ca53b55f26c439bb931ea7185708be3e64fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{sharedDriveItem-id}"].DriveItem
    .Request()
    .Expand("children")
    .GetAsync();

```