---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc10a946c80d450af74f0704e06e7c24963e5528344ca065567c40a2d172c59e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162813"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.planner().rosters("523a9d5a-f9d5-45c1-929f-b8525393515c").members("5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38")
    .buildRequest()
    .delete();

```