---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed831c7543d839f12e566de47a4965d8d8a045ba22228a76d0e4921eab728302
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Request()
    .DeleteAsync();

```