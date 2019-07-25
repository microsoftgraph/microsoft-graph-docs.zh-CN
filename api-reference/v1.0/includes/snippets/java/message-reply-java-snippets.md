---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 202089d03d526a7a7cd043b633ca456093b3a013
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856273"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

graphClient.me().messages("{id}")
    .reply(comment)
    .buildRequest()
    .post();

```