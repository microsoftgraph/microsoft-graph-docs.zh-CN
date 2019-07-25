---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d49831ad9b607d79c0c6c48e1985992d2c9e169
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870631"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = graphClient.schemaExtensions("graphlearn_test")
    .buildRequest()
    .get();

```