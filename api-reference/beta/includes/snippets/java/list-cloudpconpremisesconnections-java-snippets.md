---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a2bae6948726bd19a3c74ff5fd8b9619b6d0156eb1e8e3c3a209bcd4094866f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333063"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnectionCollectionPage onPremisesConnections = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections()
    .buildRequest()
    .get();

```