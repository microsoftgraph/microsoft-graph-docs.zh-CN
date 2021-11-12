---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5f66fd7becf1ad6ff681c201639500ef796a79f54f4e68d8f88b4943bcd9ae3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Contacts["{orgContact-id}"].Manager
    .Request()
    .GetAsync();

```