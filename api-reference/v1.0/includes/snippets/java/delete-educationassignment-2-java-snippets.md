---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b698347f637c8d187703491496753a031b9bbe696c2dbf468c54ea928304843
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274260"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("c42f493f-42b4-4e7d-8148-af894cbc518b").assignmentCategories("b93d3b6b-360c-45c0-8764-e8bb622a9504")
    .buildRequest()
    .delete();

```