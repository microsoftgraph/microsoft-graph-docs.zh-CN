---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55b126cd8046ceb073089fc12c725fb653751c11c82397e3688facdc3efece3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .Send()
    .Request()
    .PostAsync();

```