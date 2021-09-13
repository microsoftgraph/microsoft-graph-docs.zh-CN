---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ffb5a45a8c14f380fc4ec001b16cb42dc878e145fa68ef4d2b146aea1dfdfad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332391"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().patents("{id}")
    .buildRequest()
    .delete();

```