---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e847b42b96f687f4a36690e78aece0988549c06d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864820"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call Call = graphClient.app().calls("{id}")
    .buildRequest()
    .get();

```