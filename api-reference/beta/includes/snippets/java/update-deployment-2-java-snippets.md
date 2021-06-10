---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27fa021913bacb67e84a2baf5e235f1ae32ce2e4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Deployment deployment = new Deployment();
WindowsDeploymentSettings settings = new WindowsDeploymentSettings();
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

graphClient.admin().windows().updates().deployments("b5171742-1742-b517-4217-17b5421717b5")
    .buildRequest()
    .patch(deployment);

```