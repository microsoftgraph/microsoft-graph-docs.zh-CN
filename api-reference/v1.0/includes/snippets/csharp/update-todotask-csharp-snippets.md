---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 563586e1fd834c8c907a5601e58a98c85786bf06
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2020-07-25T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Todo.Lists["AAMkADA1MTHgwAAA="].Tasks["721a35e2-35e2-721a-e235-1a72e2351a72"]
    .Request()
    .UpdateAsync(todoTask);

```