---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05d964b51281da9d6e9dd4f80ce18875450aaa00
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageCollectionPage accessPackages = graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .get();

```