---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b1dcc7d6f82299bcf56d34ad586f308237fd5e87f4952bb19e64b8a79b56068
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .delete();

```