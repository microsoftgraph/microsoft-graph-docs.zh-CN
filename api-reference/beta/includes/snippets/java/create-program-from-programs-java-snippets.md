---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04fe07fcda2aa7ed44e13f0505f5fce1e87eba043588df50120ebe85b11f8d6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106276"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Program program = new Program();
program.displayName = "testprogram3";
program.description = "test description";

graphClient.programs()
    .buildRequest()
    .post(program);

```