---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77b0f7e89738ffc78069a9121dab24ceb721bffc
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384501"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Groups["{group-id}"].Members
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Pr")
    .Select("displayName,id")
    .OrderBy("displayName")
    .GetAsync();

```