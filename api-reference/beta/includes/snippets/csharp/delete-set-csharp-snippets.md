---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b7062a6a91d0b1c8725a89d5d50004db4d9fc79bec5b32b779840c3304da023
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TermStore.Sets["{termStore.set-id}"]
    .Request()
    .DeleteAsync();

```