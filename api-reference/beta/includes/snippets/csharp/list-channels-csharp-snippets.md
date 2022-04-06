---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99825053ed9f83a28e5e0772f574eb93f5dd5fa1e81fa8c0e3a0519a66c24fc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{team-id}"].Channels
    .Request()
    .GetAsync();

```