---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2763050ca485d43c2e3efd5f6cc8c91e0c5bd2d1bbd55f9259d4c67b7646326
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219936"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTask plannerTask = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh")
    .buildRequest()
    .get();

```