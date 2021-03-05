---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74a3335870a870c034568d081b93d67240c65d11
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475104"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30")
    .buildRequest()
    .get();

```