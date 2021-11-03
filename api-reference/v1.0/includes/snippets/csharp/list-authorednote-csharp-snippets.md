---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54a4d2235e1686beea958e002a734a29b9d29267
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notes = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .GetAsync();

```