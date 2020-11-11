---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8cf7f938dc23b60b7da2a03c0de6a3bd8f8143b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

graphClient.servicePrincipals("{id}")
    .removePassword(keyId)
    .buildRequest()
    .post();

```