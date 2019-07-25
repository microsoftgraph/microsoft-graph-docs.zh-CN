---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 976585cea150c1f2863c9acbe19c452732de788a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875421"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.programs("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .delete();

```