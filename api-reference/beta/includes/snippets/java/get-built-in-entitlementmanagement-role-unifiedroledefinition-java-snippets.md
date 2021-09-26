---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78492b879b40e76b4a85e9b02ed8f9a504e43a7a15aacc0660da3e9ebe77f37c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158347"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = graphClient.roleManagement().entitlementManagement().roleDefinitions("ba92d953-d8e0-4e39-a797-0cbedb0a89e8")
    .buildRequest()
    .get();

```