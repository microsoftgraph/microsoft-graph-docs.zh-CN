---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59a3add2c77503b29e6781a3400d19352d98ba681307677e4f29b4628b96c7e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCurrencies = await graphClient.BookingCurrencies
    .Request()
    .GetAsync();

```