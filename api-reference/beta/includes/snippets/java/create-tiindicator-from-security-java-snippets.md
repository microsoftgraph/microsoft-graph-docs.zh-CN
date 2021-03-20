---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24d18a13014095bb3d106c11ea3e2a0db5cb7d83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975954"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.action = TiAction.ALERT;
LinkedList<String> activityGroupNamesList = new LinkedList<String>();
tiIndicator.activityGroupNames = activityGroupNamesList;
tiIndicator.confidence = 0;
tiIndicator.description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.";
tiIndicator.expirationDateTime = OffsetDateTimeSerializer.deserialize("2019-03-01T21:43:37.5031462+00:00");
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