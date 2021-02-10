---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d065f97bb96713a0da7908726e891c0fa6d00795
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Schools["10002"].Classes
    .Request()
    .GetAsync();

```