---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2531762afe8bba8a1ba60ee538c1bbeae482b978
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceComplianceCollectionPage managedDeviceCompliances = graphClient.tenantRelationships().managedTenants().managedDeviceCompliances()
    .buildRequest()
    .get();

```