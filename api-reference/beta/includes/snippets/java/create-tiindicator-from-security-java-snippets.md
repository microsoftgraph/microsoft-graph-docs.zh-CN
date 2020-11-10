---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf210a66aabd90387eeff1b02c198a1710cd952f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981467"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.action = TiAction.ALERT;
LinkedList<String> activityGroupNamesList = new LinkedList<String>();
tiIndicator.activityGroupNames = activityGroupNamesList;
tiIndicator.confidence = 0;
tiIndicator.description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.";
tiIndicator.expirationDateTime = CalendarSerializer.deserialize("2019-03-01T21:43:37.5031462+00:00");
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