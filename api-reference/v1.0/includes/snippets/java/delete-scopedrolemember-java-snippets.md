---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7de2cbffdf0edf84e5c724b2267db8ec53d6936
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223664"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .delete();

```