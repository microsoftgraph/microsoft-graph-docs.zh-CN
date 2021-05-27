---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ce2fe8b4ee4a285e612b519bbdd742f5e41dd32
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAssetCollectionPage members = graphClient.admin().windows().updates().deployments("{deploymentId}").audience().members()
    .buildRequest()
    .get();

```