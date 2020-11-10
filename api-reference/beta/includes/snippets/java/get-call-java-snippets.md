---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 873d875c4835b859c195f68c809f0d56c430c4ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959731"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("2f1a1100-b174-40a0-aba7-0b405e01ed92")
    .buildRequest()
    .get();

```