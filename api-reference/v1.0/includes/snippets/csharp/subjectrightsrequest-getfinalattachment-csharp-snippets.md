---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a713e553250b07bfdebefa4ca269fa005044cca
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .GetFinalAttachment()
    .Request()
    .GetAsync();

```