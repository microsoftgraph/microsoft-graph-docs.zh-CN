---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8117fad5945a9deddc6ce851fb09305a5306e33a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Request()
    .DeleteAsync();

```