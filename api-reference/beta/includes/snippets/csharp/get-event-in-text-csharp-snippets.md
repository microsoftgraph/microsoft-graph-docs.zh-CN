---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ef9ca1ed7489f6b6dc8fa275487e80ee9ed218e4250fb75660386e138a3a134
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162906"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["{event-id}"]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview")
    .GetAsync();

```