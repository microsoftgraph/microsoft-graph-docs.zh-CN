---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abefd591c20f5cc36f402702e6583bf0d642330774f3114fcd3f741679d0237d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    IsLocked = true
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .UpdateAsync(conversationThread);

```