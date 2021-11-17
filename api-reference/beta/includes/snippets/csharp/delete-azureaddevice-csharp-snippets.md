---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 062cb6bcfc5f407623297b24a86b320545218f4ab8d299581f7a66b52bf13586
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .Request()
    .DeleteAsync();

```