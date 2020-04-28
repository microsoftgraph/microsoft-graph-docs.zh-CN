---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eee5ca04d0b00eeafce73e6646377eb50b023915
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805376"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .delete();

```