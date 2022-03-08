---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 299e254d7893eb75ea426679a2f67e718a4553e2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338922"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.search().bookmarks("{bookmarkId}")
    .buildRequest()
    .delete();

```