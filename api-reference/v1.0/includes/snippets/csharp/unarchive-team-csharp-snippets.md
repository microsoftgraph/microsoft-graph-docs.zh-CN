---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65abc3057ade0ac9e89f5e3b6c2f43163675b7c7b866dad5ae7dcb8daff5307d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .Unarchive()
    .Request()
    .PostAsync();

```