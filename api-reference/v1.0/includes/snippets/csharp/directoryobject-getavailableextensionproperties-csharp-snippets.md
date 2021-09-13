---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36892b553100a28afa42bcebfbfa716309d4139fa8d41d4afb37e43216ef3493
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var isSyncedFromOnPremises = false;

await graphClient.DirectoryObjects
    .GetAvailableExtensionProperties(isSyncedFromOnPremises)
    .Request()
    .PostAsync();

```