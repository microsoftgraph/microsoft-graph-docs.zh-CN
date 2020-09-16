---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 563586e1fd834c8c907a5601e58a98c85786bf06
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843074"
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