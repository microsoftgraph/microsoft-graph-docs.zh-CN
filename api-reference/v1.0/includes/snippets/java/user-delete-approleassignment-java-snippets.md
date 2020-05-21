---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fac5dfd1f67269eee9e96bd0a1228e70b370af6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```