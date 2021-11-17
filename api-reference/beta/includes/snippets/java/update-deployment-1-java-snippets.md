---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da232850992b778235d6156d3a2ce9e02889431ee273c6d746c9d56d17d03a25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220473"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Deployment deployment = new Deployment();
DeploymentState state = new DeploymentState();
state.requestedValue = RequestedDeploymentStateValue.PAUSED;
deployment.state = state;

graphClient.admin().windows().updates().deployments("b5171742-1742-b517-4217-17b5421717b5")
    .buildRequest()
    .patch(deployment);

```