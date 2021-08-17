---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45d8c99da35767dd47325cac9e29736eedb26a48a0dcc21d70f10d5e7a6215f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = graphClient.education().classes("5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5").assignments("1fdf61ee-c129-4960-9b7c-8df159aa64b0")
    .buildRequest()
    .get();

```