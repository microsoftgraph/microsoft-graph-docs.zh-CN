---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e3df12ea0a3817f3c1585955f06645a8600d102
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428858"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream stream = graphClient.customRequest("/me/onenote/resources/{id}/content", Stream.class)
    .buildRequest()
    .get();

```