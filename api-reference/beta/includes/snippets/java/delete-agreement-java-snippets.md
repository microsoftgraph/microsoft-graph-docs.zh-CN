---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b796206811b43f296cf1b7fc25fda901c14cbcbb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962485"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.agreements("{id}")
    .buildRequest()
    .delete();

```