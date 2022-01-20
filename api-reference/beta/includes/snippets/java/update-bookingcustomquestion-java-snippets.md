---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9320b49bef178ea7885242e0674fd852e820eb3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094537"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomQuestion bookingCustomQuestion = new BookingCustomQuestion();
bookingCustomQuestion.displayName = "What is your age?";
bookingCustomQuestion.answerInputType = AnswerInputType.TEXT;
LinkedList<String> answerOptionsList = new LinkedList<String>();
bookingCustomQuestion.answerOptions = answerOptionsList;

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customQuestions("3bc6fde0-4ad3-445d-ab17-0fc15dba0774")
    .buildRequest()
    .patch(bookingCustomQuestion);

```