---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24cfdf0afcf059ec2623a3e7b3529968eb78213a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Plans["xqQg5FS2LkCp935s-FIFm2QAFkHM"].Tasks
    .Request()
    .GetAsync();

```