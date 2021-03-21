---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c21c21338a0c539fada579586206803cfb9cbf6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .delete();

```