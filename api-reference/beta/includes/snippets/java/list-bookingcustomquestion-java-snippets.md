---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04cfaa5efdc233062e853bef35fa7b0072ee2ba
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114038"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomQuestionCollectionPage customQuestions = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customQuestions()
    .buildRequest()
    .get();

```