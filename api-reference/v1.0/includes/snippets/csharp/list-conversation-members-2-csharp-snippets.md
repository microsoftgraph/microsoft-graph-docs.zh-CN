---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41dcdfd79044e64ca6bd68ad17617f7c51f9405e2a3eabae794f69387215ada9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Chats["{chat-id}"].Members
    .Request()
    .GetAsync();

```