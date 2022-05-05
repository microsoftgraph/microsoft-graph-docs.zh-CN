---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4689dd12f8b77e81c0a996205148c92a74fecb47
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220255"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "testProperties";

graphClient.applicationTemplates("8adf8e6e-67b2-4cf2-a259-e3dc5476c621")
    .instantiate(ApplicationTemplateInstantiateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .build())
    .buildRequest()
    .post();

```