---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2366c967c24a761b6693ae8f7efd5d63496d6272a1a401dcec91106bbcc9fc03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Groups["{termStore.group-id}"]
    .Request()
    .DeleteAsync();

```