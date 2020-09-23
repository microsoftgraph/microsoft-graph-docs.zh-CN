---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f30b48389f13273a803af94cfb89e7c3095678b2
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223484"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .get();

```