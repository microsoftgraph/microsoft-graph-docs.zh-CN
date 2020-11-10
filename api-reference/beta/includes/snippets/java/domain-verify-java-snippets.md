---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24ea5c405f77150715d195785a0707a030c4a18a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .verify()
    .buildRequest()
    .post();

```