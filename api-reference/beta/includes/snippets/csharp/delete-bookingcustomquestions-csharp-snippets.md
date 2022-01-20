---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f220c99b5c3e9ea4825c2696e8102ebddff5edc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106804"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].CustomQuestions["{bookingCustomQuestion-id}"]
    .Request()
    .DeleteAsync();

```