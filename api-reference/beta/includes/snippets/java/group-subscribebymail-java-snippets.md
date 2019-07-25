---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c7320969d2dddf5874cf94b930311de4f507202
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857925"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .subscribeByMail()
    .buildRequest()
    .post();

```