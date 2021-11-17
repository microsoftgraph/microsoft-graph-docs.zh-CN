---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9655409e2574ec00d35146acf52488c036b2f6ea906415c0cb505898c9f1908
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
    .instantiate(ApplicationTemplateInstantiateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .build())
    .buildRequest()
    .post();

```