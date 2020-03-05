---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 755cb13874c60a38476ddd1e2e8f7ef1f6dfaaa3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Outlook.TaskFolders["AAMkADIyAAAhrbPWAAA="].Tasks
    .Request()
    .GetAsync();

```