---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd7087f75f2fad30cdbbebb0731ef5e50136cbee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968386"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = graphClient.me().profile().awards("{id}")
    .buildRequest()
    .get();

```