---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b41e6bc6d44fcfb26ab764d91a698365655bab23266b46e6707bdbb79a2603f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105302"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .GetAsync();

```