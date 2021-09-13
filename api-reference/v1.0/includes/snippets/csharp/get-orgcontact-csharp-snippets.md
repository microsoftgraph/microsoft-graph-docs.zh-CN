---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd8d122392c6051fc8351ac7cefb939d2d50e575f1bce101f1ba3d8701ab743b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .GetAsync();

```