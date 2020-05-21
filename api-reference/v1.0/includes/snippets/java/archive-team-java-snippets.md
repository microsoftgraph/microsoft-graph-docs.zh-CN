---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43c3ca6da1b50ddf294d0f7520592f2db1f64f8c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335731"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .archive(null)
    .buildRequest()
    .post();

```