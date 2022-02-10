---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a388dc3d9d5830fe65b9e520276a3f4d810cb425
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("x509Certificate")
    .buildRequest()
    .delete();

```