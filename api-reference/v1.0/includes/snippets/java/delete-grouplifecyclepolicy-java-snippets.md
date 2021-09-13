---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0eef2e97114bb0695ae6cec84c3c9a4f4256c32391e099d503bfc81d8ca5b3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groupLifecyclePolicies("{id}")
    .buildRequest()
    .delete();

```