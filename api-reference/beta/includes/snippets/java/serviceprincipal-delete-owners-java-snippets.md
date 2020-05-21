---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6b20029241864d7dd5e4934e0b9a70b252a2967
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333793"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.serviceprincipals("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```