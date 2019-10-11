---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cce21d76fa59fa37ca9493498a342f58043622b1
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428825"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream stream = graphClient.customRequest("/me/drive/items/{item-id}/versions/{version-id}/content", Stream.class)
    .buildRequest()
    .get();

```