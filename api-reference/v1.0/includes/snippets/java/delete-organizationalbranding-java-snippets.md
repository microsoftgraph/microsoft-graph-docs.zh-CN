---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eed7353132e065bc565c03a6afcf2f9d4f79e0d7
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("84841066-274d-4ec0-a5c1-276be684bdd3").branding()
    .buildRequest()
    .delete();

```