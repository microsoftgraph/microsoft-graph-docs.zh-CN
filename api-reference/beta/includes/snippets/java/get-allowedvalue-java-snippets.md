---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fec0cebed46e93c3afe5f724fef343d260243820
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224308"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AllowedValue allowedValue = graphClient.directory().customSecurityAttributeDefinitions("Engineering_Project").allowedValues("Alpine")
    .buildRequest()
    .get();

```