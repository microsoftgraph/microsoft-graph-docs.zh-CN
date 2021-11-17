---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c78352adf9cbaca49f264aafb3186668f8d750173e254a8d127a42e14e500d06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105047"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusinesses = await graphClient.BookingBusinesses
    .Request()
    .GetAsync();

```