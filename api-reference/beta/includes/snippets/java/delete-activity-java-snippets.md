---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17b1f1708426909dca42d5c36a222d070a8be79d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().activities("13881113971988980728")
    .buildRequest()
    .delete();

```