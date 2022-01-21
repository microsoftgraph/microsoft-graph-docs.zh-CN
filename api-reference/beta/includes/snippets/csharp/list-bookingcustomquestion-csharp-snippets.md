---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9473a89792ddbc10c0ad2920d7634fb6487b786
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customQuestions = await graphClient.BookingBusinesses["{bookingBusiness-id}"].CustomQuestions
    .Request()
    .GetAsync();

```