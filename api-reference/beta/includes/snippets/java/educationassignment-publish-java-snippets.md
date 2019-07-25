---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3dda599cff6e8515d6f02e00de45c814fd0e276e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860773"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002")
    .publish()
    .buildRequest()
    .post();

```