---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dcd96836de0a60ebb1c716239cf6316b6febcb2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("c42f493f-42b4-4e7d-8148-af894cbc518b").assignmentCategories("b93d3b6b-360c-45c0-8764-e8bb622a9504")
    .buildRequest()
    .delete();

```