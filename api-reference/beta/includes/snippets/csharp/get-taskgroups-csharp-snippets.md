---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da774161f38bf9055c74974e01f8f08a1cfddd15c38b996f23d36cb6a17c2a52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskGroups = await graphClient.Me.Outlook.TaskGroups
    .Request()
    .GetAsync();

```