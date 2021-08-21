---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f8d7c732896bbc595c0f071bc109036f6bc8f2ec8c3c627701ff40e2c061b08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.PrivilegedAccess["{privilegedAccess-id}"].Resources
    .Request()
    .GetAsync();

```