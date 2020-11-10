---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1617b18c6e69e9769bc9b9345e78040728f0bc25
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971212"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .disableSmsSignIn()
    .buildRequest()
    .post();

```