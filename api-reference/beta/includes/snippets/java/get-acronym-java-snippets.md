---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e2f5a4ba6f23b5e20b85d1f491005f82452a805
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Acronym acronym = graphClient.search().acronyms("{acronymsId}")
    .buildRequest()
    .get();

```