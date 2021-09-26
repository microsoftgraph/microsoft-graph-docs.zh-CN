---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0622bc35777ddc42bca57c784c7adc20b8e387e3cfb35e01954e11298d6749e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .runHealthChecks()
    .buildRequest()
    .post();

```