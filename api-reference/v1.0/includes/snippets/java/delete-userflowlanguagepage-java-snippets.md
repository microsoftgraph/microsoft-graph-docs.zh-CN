---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e98e904c3e15f2b1aa751870bb379ba587f7ad4be96699cef5d868f20d9c55c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162529"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").overridesPages("selfasserted1_1").content()
    .buildRequest()
    .delete();

```