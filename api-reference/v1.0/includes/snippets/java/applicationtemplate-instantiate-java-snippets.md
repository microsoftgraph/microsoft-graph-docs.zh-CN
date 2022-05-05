---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7865d81ab7755006db1ddf72dfc5e08d2aebdce1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220331"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Azure AD SAML Toolkit";

graphClient.applicationTemplates("229946b9-a9fb-45b8-9531-efa47453ac9e")
    .instantiate(ApplicationTemplateInstantiateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .build())
    .buildRequest()
    .post();

```