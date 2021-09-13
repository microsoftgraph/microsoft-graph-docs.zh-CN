---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e3804e5e522a88cb21b242535f131b8c324124fc341168bbcba54e171f4440c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"]
    .Request()
    .DeleteAsync();

```