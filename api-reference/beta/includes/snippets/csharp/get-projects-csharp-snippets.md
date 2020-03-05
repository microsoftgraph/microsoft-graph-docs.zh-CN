---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31a10957ab03559dce7401bd10a084a1aed7604b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996865"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projects = await graphClient.Me.Profile.Projects
    .Request()
    .GetAsync();

```