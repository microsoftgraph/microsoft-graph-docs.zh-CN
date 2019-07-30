---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d86de3dd36f93d93966bc6e4f4e9d550dfb8deb
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Drive.Bundles["{bundle-id}"]
    .Request()
    .GetAsync();

```