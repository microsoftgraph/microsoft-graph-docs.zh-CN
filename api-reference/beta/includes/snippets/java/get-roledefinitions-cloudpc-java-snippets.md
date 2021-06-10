---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ac0207bab741e229a474908d15fe024f2eedec3
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().cloudPC().roleDefinitions()
    .buildRequest()
    .get();

```