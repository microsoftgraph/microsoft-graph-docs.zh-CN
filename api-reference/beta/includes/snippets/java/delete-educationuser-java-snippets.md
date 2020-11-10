---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1474c5ca083e61de9a6de7d471060316699470de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955320"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("13019")
    .buildRequest()
    .delete();

```