---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92b6c5c8cf75b3a7d90dff2975f4f15f88aa831f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224588"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinitionCollectionPage customSecurityAttributeDefinitions = graphClient.directory().customSecurityAttributeDefinitions()
    .buildRequest()
    .filter("attributeSet eq 'Engineering' and status eq 'Available' and type eq 'String'")
    .get();

```