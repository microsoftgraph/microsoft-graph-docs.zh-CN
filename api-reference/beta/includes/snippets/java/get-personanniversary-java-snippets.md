---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c5e8a3a03b2d635b48f22ad48093457f1133a87
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500484"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .get();

```