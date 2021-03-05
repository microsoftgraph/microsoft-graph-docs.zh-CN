---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eb6b5a5663c17f115e16ca5bc2f1dd2826c752a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475318"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("microsoftAuthenticator")
    .buildRequest()
    .delete();

```