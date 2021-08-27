---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab903ce9c58b4192dd62b0f33da8f1b1102a7e4aac368d85377981d8e058b7c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .Top(2)
    .GetAsync();

```