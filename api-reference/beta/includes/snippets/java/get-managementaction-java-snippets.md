---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a89e538135ed4e7c59bff7938a03049c50fa1ed8028f10c78c7c7309782c3687
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementAction managementAction = graphClient.tenantRelationships().managedTenants().managementActions("{managementActionId}")
    .buildRequest()
    .get();

```