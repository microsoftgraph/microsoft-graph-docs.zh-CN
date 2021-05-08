---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fd1574b74f30b89a33106b72978cb556af4d634
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239186"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Deployment deployment = new Deployment();
FeatureUpdateReference content = new FeatureUpdateReference();
content.version = "20H2";
deployment.content = content;
WindowsDeploymentSettings settings = new WindowsDeploymentSettings();
RolloutSettings rollout = new RolloutSettings();
rollout.devicesPerOffer = 100;
settings.rollout = rollout;
MonitoringSettings monitoring = new MonitoringSettings();
LinkedList<MonitoringRule> monitoringRulesList = new LinkedList<MonitoringRule>();
MonitoringRule monitoringRules = new MonitoringRule();
monitoringRules.signal = MonitoringSignal.ROLLBACK;
monitoringRules.threshold = 5;
monitoringRules.action = MonitoringAction.PAUSE_DEPLOYMENT;
monitoringRulesList.add(monitoringRules);
monitoring.monitoringRules = monitoringRulesList;
settings.monitoring = monitoring;
deployment.settings = settings;

graphClient.admin().windows().updates().deployments()
    .buildRequest()
    .post(deployment);

```