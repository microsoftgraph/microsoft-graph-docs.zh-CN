---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96e75c43723d1308ac0a54db608594f75624371b
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223282"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .delete();

```