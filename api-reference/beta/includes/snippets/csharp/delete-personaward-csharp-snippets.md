---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97ff70527f7c650480c0121394ea69761287b7692f4e11bb428584480be31488
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Awards["{personAward-id}"]
    .Request()
    .DeleteAsync();

```