---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6874fbb795516a9b30c17a3fdad199503424fafe
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodConfiguration authenticationMethodConfiguration = graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("x509Certificate")
    .buildRequest()
    .get();

```