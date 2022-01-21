---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c9a25e24d18a5d93679e1bcba103b6b767991b1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomQuestion = new BookingCustomQuestion
{
    DisplayName = "What is your age?",
    AnswerInputType = AnswerInputType.Text,
    AnswerOptions = new List<String>()
    {
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].CustomQuestions["{bookingCustomQuestion-id}"]
    .Request()
    .UpdateAsync(bookingCustomQuestion);

```