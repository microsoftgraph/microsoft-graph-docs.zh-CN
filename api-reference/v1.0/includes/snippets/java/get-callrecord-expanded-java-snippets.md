---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84c5384a2b1147eb87b07451ef27c40f978226df
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("{id}")
    .buildRequest()
    .expand("sessions($expand=segments)")
    .get();

```