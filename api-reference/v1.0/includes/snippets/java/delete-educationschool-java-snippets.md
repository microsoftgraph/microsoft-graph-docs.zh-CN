---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f2811f24f521afc88970ade8765816f657376b9d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887761"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}")
    .buildRequest()
    .delete();

```