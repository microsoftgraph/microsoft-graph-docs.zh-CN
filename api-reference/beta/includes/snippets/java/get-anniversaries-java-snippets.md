---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e3e9948a46b0c5a19b70e1d86fae75e2a84e5b9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500552"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonAnnualEventCollectionPage anniversaries = graphClient.me().profile().anniversaries()
    .buildRequest()
    .get();

```