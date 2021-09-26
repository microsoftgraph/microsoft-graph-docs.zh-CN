---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6a596250b3b812d626e2437616aab1825757825d1b50f26227a21a58341d08f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().entitlementManagement().roleDefinitions()
    .buildRequest()
    .get();

```