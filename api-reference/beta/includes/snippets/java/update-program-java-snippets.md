---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a3d7384699ea2deb4f68a41a6992eec15a8c9c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875363"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Program program = new Program();
program.displayName = "testprogram3 new name";

graphClient.programs("7e59d237-2fb0-4e5d-b7bb-d4f9f9129213")
    .buildRequest()
    .patch(program);

```