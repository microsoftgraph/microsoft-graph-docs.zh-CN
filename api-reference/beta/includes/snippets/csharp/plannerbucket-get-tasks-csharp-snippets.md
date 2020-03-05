---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba0068cccad052aefb22cee907db310bde7e00ea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Planner.Buckets["gcrYAaAkgU2EQUvpkNNXLGQAGTtu"].Tasks
    .Request()
    .GetAsync();

```