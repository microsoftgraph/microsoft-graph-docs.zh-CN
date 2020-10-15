---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa1bcd19904885dca777b0f1800bc2afc05dc8f9
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462552"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.subscriptions("7f105c7d-2dc5-4530-97cd-4e7ae6534c07")
    .buildRequest()
    .delete();

```