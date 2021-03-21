---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae4562af14e885169414d6b474cd73dba930936b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969588"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .delete();

```