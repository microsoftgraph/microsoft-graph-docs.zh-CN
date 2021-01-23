---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0c318dcf4beba1c0d2db95755e06ceba65fdb18
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945439"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11014"].Assignments["19002"]
    .Request()
    .DeleteAsync();

```