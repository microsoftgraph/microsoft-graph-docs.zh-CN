---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5753fa990c5c61564a54bb27e1119f3dc22769eff952e8112276279604c385c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{device-id}"].RegisteredUsers["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```