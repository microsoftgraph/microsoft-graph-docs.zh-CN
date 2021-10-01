---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b26513d582ace9c097d8e8232691da4eea5d60ce4b7b91b9b602e52e3d6aaef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfile = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Request()
    .GetAsync();

```