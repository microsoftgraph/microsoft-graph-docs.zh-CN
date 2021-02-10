---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d5e4ee5614d6d21a640457b49f6876008a9273d
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{id}"].Teachers["14012"]
    .Request()
    .DeleteAsync();

```