---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62a0cdb09ce335b7b3cac1996b104fbea5b0bcba
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919966"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp")
    .buildRequest()
    .get();

```