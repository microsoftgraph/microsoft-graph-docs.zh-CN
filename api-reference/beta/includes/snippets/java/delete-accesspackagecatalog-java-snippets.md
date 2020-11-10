---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 404f9e2d804c55f0e9984d0d3e047f60cee5c889
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951982"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}")
    .buildRequest()
    .delete();

```