---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18a9b1396c5f0d3aea0025d2d995171c9f14f63b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871126"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScreenSharingRole role = ScreenSharingRole.VIEWER;

graphClient.communications().calls("{id}")
    .changeScreenSharingRole(role)
    .buildRequest()
    .post();

```