---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3b206bbf66b3396aff47085f29c2cac482881ea
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951926"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageResourceCollectionPage accessPackageResources = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}").accessPackageResources()
    .buildRequest()
    .get();

```