---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a0add8657c731f275e2c56201c12e8d8b5dab84d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174706"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.action = TiAction.ALERT;
LinkedList<String> activityGroupNamesList = new LinkedList<String>();
tiIndicator.activityGroupNames = activityGroupNamesList;
tiIndicator.confidence = 0;
tiIndicator.description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.";
tiIndicator.expirationDateTime = "2019-03-01T21:43:37.5031462+00:00";
tiIndicator.externalId = "Test--8586509942679764298MS501";
tiIndicator.fileHashType = FileHashType.SHA256;
tiIndicator.fileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313";
LinkedList<String> killChainList = new LinkedList<String>();
tiIndicator.killChain = killChainList;
LinkedList<String> malwareFamilyNamesList = new LinkedList<String>();
tiIndicator.malwareFamilyNames = malwareFamilyNamesList;
tiIndicator.severity = 0;
LinkedList<String> tagsList = new LinkedList<String>();
tiIndicator.tags = tagsList;
tiIndicator.targetProduct = "Azure Sentinel";
tiIndicator.threatType = "WatchList";
tiIndicator.tlpLevel = TlpLevel.GREEN;

graphClient.security().tiIndicators()
    .buildRequest()
    .post(tiIndicator);

```