---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0403e3d4bdb92878967265e9a0183af6e2bb755cabdebe6a8d5f3a8cbabd675
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161345"
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