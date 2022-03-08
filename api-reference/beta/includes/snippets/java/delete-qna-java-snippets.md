---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c47149ddc9e696c6c1f7c4efe43be975fbc6530
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338933"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.search().qnas("{qnaId}")
    .buildRequest()
    .delete();

```