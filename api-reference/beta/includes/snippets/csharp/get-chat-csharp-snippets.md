---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39b1c2db4bcf38c17f178e71a8ee0489e1d59a6b
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119718"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{id}"].Chats["{id}"]
    .Request()
    .GetAsync();

```