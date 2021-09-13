---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dea5f6a5f84c05a10c5c052993f0f154f991483f98d7b30a87a3e918b7ab2b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Drive
    .Recent()
    .Request()
    .GetAsync();

```