---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53e4b5810360244bfa4d69e5adf8f5ad54d7b611
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalCollectionPage servicePrincipal = graphClient.groups("3802e9bb-0951-4e18-b9eb-f934b4241194").members().microsoft.graph.servicePrincipal()
    .buildRequest()
    .get();

```