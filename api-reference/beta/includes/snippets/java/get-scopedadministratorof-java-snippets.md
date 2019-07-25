---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2e6c8cd096dcedd6735f71405042598f3d9c9e58
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867074"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content scopedAdministratorOf = graphClient.me().scopedAdministratorOf()
    .buildRequest()
    .get();

```