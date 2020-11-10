---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cda11b9c9df5692b5012d2d2047c5943dab2a04b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961343"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethod authenticationMethod = graphClient.me().authentication().methods("{id}")
    .buildRequest()
    .get();

```