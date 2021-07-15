---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca2bf7a880cc45aaa75426dbbbd422c72dd26675
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443047"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementTemplateCollectionPage managementTemplates = graphClient.tenantRelationships().managedTenants().managementTemplates()
    .buildRequest()
    .get();

```