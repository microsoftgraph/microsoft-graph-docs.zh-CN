---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9abae5465d74928e9c1c80db15df3995a64d0b23
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shiftPreferences = await graphClient.Users["871dbd5c-3a6a-4392-bfe1-042452793a50"].ShiftPreferences
    .Request()
    .GetAsync();

```