---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37893e69d08d73e7ac94cf423649f2b4f77dc168
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222843"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").participants("{id}")
    .buildRequest()
    .delete();

```