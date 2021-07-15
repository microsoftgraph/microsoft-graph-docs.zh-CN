---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6f34262ca470a69ce8547348acf313a3576aa9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441439"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementTemplate managementTemplate = graphClient.tenantRelationships().managedTenants().managementTemplates("{managementTemplateId}")
    .buildRequest()
    .get();

```