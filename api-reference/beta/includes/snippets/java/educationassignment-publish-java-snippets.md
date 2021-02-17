---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a8b2d730b410964b8fe02fc5ca0485b4cc25234
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274854"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.education().classes("11012").assignments("19002")
    .getResourcesFolderUrl()
    .buildRequest()
    .get();

```