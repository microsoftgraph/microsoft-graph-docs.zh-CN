---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c905b410432d3d7870d53f6a87b9779cb475b5d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Shared legal agreements"
};

await graphClient.Drive.Items["{bundle-id}"]
    .Request()
    .UpdateAsync(driveItem);

```