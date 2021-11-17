---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63e8c6b3d6cbe2e5673bc88c85a7a9958128ff2a5e7ed3d507d9fe4378363fb5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .delete();

```