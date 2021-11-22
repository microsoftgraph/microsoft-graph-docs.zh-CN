---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9e049af6d71e647faf4e91fcd32b5c3718219eb27749437ef6975aea6b7efd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Request()
    .DeleteAsync();

```