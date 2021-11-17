---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d792e2fd99dbdd6dda6cc36a343b17bff61a95ad845e440fc3d60740e6e684e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218531"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .delete();

```