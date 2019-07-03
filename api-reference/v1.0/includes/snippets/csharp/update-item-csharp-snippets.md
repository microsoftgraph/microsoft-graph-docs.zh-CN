---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ddda186db43dbca0da561091ca038b7f72aee737
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509585"
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