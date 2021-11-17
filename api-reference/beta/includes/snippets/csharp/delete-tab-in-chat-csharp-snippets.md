---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e10c588ada7b81fdecfb3efcbdcfc84e9a64d42d12a7a975843d86db1946c02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278347"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .DeleteAsync();

```