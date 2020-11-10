---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f9eb72c1a3285f66c2617c89a3a062852df7606
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976273"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===").extensions("Com.Contoso.Referral")
    .buildRequest()
    .delete();

```