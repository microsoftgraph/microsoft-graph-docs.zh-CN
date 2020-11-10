---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6e1b2b4e56154ff75a175f911a1803b74c46197
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981601"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}").mentions("{id}")
    .buildRequest()
    .delete();

```