---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7aa2eba808e43b9a1693012db833da487ab6b80
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865282"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").staffMembers("5fae928f-6d2d-417a-ad96-4b0caeb362d6")
    .buildRequest()
    .delete();

```