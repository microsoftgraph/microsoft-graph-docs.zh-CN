---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3bab0ad06a3f204b9a7d8e8a237501940f87d48d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881822"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "edit";

String scope = "organization";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope)
    .buildRequest()
    .post();

```