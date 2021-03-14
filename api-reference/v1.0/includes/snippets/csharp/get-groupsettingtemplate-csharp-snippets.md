---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1622470cc860859a42906163355ff37fd7d59576
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettingTemplate = await graphClient.GroupSettingTemplates["{groupSettingTemplate-id}"]
    .Request()
    .GetAsync();

```