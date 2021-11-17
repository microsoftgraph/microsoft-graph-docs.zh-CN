---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d3417f07e69602eada3d9a11ca312c37fef807d4178a6e233eaef06f2d7d9da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .delete();

```