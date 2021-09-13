---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ad302717d63e2c9d8e6748583184f8d1b31fdcd287296c5e621ba7662e878e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Manager.Reference
    .Request()
    .PutAsync("{id}");

```