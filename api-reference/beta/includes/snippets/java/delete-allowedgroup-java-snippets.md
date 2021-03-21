---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeeaa6908c895e8a8b4bd36e1b4595f4313bf40f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967006"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{id}").allowedGroups("{id}").reference()
    .buildRequest()
    .delete();

```