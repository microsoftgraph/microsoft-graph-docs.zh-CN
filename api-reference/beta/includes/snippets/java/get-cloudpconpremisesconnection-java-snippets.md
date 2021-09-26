---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 715d091276dc45bc2a9ab0a8e55165f58112397c9743e14870709e914b2074d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105237"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnection cloudPcOnPremisesConnection = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .buildRequest()
    .get();

```