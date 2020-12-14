---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4edb53353751fb73c8334ea6fc0e4da03cf655d2
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49656997"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("{id}").teamwork().installedApps("{id}").chat()
    .buildRequest()
    .get();

```