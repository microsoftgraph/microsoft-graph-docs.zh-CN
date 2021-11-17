---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7ce3856abbab906c36ebe8d992b7062a023d689a4ff4466ce415aabd8df1a58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Phones["{itemPhone-id}"]
    .Request()
    .DeleteAsync();

```