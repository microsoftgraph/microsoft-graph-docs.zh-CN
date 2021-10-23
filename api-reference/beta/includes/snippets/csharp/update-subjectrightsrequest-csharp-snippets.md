---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1ad790e2e58b58e394bc530b81cfb0d9d0dc7b4
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequest = new SubjectRightsRequestObject
{
    InternalDueDateTime = DateTimeOffset.Parse("2021-08-30T00:00:00Z")
};

await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .Request()
    .UpdateAsync(subjectRightsRequest);

```