---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c53b1d477a0f09a9cb4a07ea6ff51213411d707
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AcronymCollectionPage acronyms = graphClient.search().acronyms()
    .buildRequest()
    .get();

```