---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 428d39095164c4d0252c8e2ba7613d0be3a795164c4df2f6618714ec7d56dc5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
};

await graphClient.Devices["{device-id}"]
    .CheckMemberObjects(ids)
    .Request()
    .PostAsync();

```