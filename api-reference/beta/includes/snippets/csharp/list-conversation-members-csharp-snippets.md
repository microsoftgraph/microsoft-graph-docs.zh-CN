---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 301c9b8c4107459ec8ef2ad92b744133517b40345d3be577082d14c7bdb4925b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Me.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```