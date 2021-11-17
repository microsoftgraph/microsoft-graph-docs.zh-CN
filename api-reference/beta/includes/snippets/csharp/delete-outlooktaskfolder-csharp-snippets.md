---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c27b6dfcd3940df7691ef5135a753f6289786d6290da255627867152c6e2f5dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105738"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"]
    .Request()
    .DeleteAsync();

```