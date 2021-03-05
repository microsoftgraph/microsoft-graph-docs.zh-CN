---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8598d2db760d3223ff186e0bf8e0fef39519e174
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475623"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .delete();

```