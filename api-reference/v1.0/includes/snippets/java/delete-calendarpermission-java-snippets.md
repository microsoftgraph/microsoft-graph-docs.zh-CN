---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 831abb1450b5ff7d4ab341d4244bebb1b237fa4a
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806620"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .delete();

```