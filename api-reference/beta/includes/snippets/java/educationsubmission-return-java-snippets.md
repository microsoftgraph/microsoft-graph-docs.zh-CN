---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4582692cf4f4e757f49845ebfa50262959b6f7a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955482"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .return()
    .buildRequest()
    .post();

```