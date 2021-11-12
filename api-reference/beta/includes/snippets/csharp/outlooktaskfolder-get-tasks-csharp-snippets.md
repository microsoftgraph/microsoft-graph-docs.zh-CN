---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 943c65def0ab2649d1607c94879c4b17a2dc9cb197fa91f43ecad61b146c620d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"].Tasks
    .Request()
    .GetAsync();

```