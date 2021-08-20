---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0cae5e3408f20883fe8af6d4f7925a1572862d9b5e6c4c2492b2bc73c54d5d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].Members["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```