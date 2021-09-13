---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f2cb4b62c28f5b6b8cfcb875ecf4eacd69e0075817380a0ba8abe084bf7dabc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Me.Schools
    .Request()
    .GetAsync();

```