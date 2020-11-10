---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab8331f01026a1d3165a7a9d02de52544922df2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952283"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.catalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128";
accessPackage.displayName = "sales reps";
accessPackage.description = "outside sales representatives";

graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .post(accessPackage);

```