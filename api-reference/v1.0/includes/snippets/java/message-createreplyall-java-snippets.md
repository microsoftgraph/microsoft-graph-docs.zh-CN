---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5e8f5e0b76435780003303d7cc2d7db0c91d622
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883176"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReplyAll()
    .buildRequest()
    .post();

```