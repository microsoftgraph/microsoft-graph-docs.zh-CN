---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d3abfd8a05d639136f02927226626e27ba760b0f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplate = await graphClient.DirectorySettingTemplates["{id}"]
    .Request()
    .GetAsync();

```