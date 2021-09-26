---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 787c7e22cc8f307522700c470f811959b63d0f79
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationSettings organizationSettings = graphClient.organization("a9f3c90b-04fd-4504-a302-47672bbca6c8").settings()
    .buildRequest()
    .get();

```