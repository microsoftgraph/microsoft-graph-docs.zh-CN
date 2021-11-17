---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5ded3e50476c3ed24089d320d7675463e64c4c05c4a8540d7a2edeb7098428f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

await graphClient.Applications["{application-id}"]
    .RemovePassword(keyId)
    .Request()
    .PostAsync();

```