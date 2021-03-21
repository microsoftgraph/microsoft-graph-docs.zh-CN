---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8abe35b2071747aa632493ef96a4ccc369c8b4c0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["{chat-id}"].Tabs
    .Request()
    .Filter("teamsApp/id eq 'com.microsoft.teamspace.tab.web'")
    .Expand("teamsApp")
    .GetAsync();

```