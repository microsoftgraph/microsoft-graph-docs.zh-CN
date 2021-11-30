---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c8217e56e57485d240aa91f9c17ff234616da49
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225761"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = graphClient.directory().customSecurityAttributeDefinitions("Engineering_ProjectDate")
    .buildRequest()
    .get();

```