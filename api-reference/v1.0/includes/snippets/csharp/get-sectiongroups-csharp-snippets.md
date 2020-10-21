---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d3ed7b57d2beec92bfa0426168c9cea33c0618f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.SectionGroups["{id}"].SectionGroups
    .Request()
    .GetAsync();

```