---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30129d9e1e0d745208f725bc78d55b872bd1b262dc191a82538acbe3e6f658d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Restore()
    .Request()
    .PostAsync();

```