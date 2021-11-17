---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d07b6ac54e9a0610c841b0c89371aa25c442d5cc435b470c9deff86a07c01346
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277776"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementIntent managementIntent = graphClient.tenantRelationships().managedTenants().managementIntents("{managementIntentId}")
    .buildRequest()
    .get();

```