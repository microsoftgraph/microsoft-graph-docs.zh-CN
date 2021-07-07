---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c843ecd6f6bea2daa8b7a5eaf0e9447d8b3c2fe5
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEventGetAuditActivityTypesCollectionPage getAuditActivityTypes = graphClient.deviceManagement().virtualEndpoint().auditEvents()
    .getAuditActivityTypes()
    .buildRequest()
    .get();

```