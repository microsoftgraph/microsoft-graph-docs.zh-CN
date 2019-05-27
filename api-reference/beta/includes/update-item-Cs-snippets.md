---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddda186db43dbca0da561091ca038b7f72aee737
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "new-file-name.docx"
};

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .UpdateAsync(driveItem);

```