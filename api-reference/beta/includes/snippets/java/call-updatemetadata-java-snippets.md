---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 780b21dc9c7584d857ac4b8281e0ad03ca484956
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864668"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String metadata = "metadata-value";

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .updateMetadata(metadata,clientContext)
    .buildRequest()
    .post();

```