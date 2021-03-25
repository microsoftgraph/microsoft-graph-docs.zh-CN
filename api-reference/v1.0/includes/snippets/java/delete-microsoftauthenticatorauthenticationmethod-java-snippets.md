---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4029a499b6077ae1ec9e433fa6cf5e6c51ee79cf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202834"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```