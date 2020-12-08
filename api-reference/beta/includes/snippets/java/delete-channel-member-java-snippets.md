---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d31e56277845dfec767479c14856be69241d36
ms.sourcegitcommit: c419bb8901b7766af193196f80bc1d497643fcb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573986"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").channels("19:56eb04e133944cf69e603c5dac2d292e@thread.skype").members("ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=")
    .buildRequest()
    .delete();

```