---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 774c14131cf7b844342dcb73cb7d8800f076f6c5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981694"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .delete();

```