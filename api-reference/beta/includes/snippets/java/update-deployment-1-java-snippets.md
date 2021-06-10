---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce6077a60707bdc2ffcb879d33a6eb94f70e2bc1
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870260"
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