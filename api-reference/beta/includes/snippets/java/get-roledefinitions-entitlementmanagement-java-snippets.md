---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20e08ce2a6e1868ea950ec371f8bac8a533010a6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().entitlementManagement().roleDefinitions()
    .buildRequest()
    .get();

```