---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26f11ba9f562f7d6a723e4ae20147f541039de98
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854585"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOrganizationSettings cloudPcOrganizationSettings = graphClient.deviceManagement().virtualEndpoint().organizationSettings()
    .buildRequest()
    .get();

```