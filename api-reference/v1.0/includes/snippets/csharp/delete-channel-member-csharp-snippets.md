---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 193019c9d335eca1ac2e4b1bfae2c47eb8bf9285cbbd078a7cc450eb0c58b1db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```