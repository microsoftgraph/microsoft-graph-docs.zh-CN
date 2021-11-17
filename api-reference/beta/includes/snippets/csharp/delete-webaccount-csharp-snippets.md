---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de51e5e9dde765a149a008c21dfb565971d9632dfae6dfd2b47c755575c9a551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163903"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.WebAccounts["{webAccount-id}"]
    .Request()
    .DeleteAsync();

```