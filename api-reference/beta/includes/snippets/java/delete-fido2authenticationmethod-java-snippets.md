---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab08c6492ca09c544b1e18b37546c2dcd646e27
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().fido2Methods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```