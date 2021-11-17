---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1247d81b21f4d490940e002c8b837f4ea68eb2f3602ce4fef813cb4d8e12a8fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903071"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUser riskyUser = graphClient.riskyUsers("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```