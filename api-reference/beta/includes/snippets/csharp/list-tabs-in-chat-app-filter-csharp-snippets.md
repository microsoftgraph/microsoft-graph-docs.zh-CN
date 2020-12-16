---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da1edf789cedc5d78086cef2248cecb00484d95a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Chats["19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"].Tabs
    .Request()
    .Filter("teamsApp/id eq 'com.microsoft.teamspace.tab.web'")
    .Expand("teamsApp")
    .GetAsync();

```