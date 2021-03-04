---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c399b8e74a4b8881e7e7a3472da422cbf2d2692
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443710"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```