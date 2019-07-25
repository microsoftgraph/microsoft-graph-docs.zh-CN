---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 45ff0b8fbc8eb0fb191e174e834a42c9c40710ed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861619"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{driveId}")
    .buildRequest()
    .get();

```