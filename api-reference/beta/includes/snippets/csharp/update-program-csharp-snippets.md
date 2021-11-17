---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d7122ca170f8a1c31f12563d85d0c478f28c3260346b4530acd4ebf4a6e15c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var program = new Program
{
    DisplayName = "testprogram3 new name"
};

await graphClient.Programs["{program-id}"]
    .Request()
    .UpdateAsync(program);

```