---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6cf78c91ba464d9c48f20dd4583b79f524044e4c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860668"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11022")
    .buildRequest()
    .delete();

```