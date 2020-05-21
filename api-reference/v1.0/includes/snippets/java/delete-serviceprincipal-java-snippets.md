---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84c5cbceae977e826c4faa3140a1db142fadf061
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334212"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .delete();

```