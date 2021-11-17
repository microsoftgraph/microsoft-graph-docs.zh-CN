---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f022e3185ce242044c26f88c7731723c16f559257151b71504264d59bf72f170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .delete();

```