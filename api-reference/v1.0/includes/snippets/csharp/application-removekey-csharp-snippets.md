---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a37edfd7c7a045c5fbca0aecd018ba9f4604b12bb7893779a850b376c88a54f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{application-id}"]
    .RemoveKey(keyId,proof)
    .Request()
    .PostAsync();

```