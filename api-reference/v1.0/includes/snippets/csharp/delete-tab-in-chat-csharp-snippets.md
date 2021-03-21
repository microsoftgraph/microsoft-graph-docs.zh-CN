---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d846f1c26b5fb7175991f6f0f0f6073af0c4e594
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .DeleteAsync();

```