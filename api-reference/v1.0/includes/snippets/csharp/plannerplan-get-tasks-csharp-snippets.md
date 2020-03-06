---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2adb3194f88ed62d8ce501b4676efef31a21e400
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Plans["{plan-id}"].Tasks
    .Request()
    .GetAsync();

```