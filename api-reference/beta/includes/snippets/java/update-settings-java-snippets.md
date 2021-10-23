---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed4303498a835f49b389a1bbb9eb6accdc6775cd
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CaseSettings caseSettings = new CaseSettings();
RedundancyDetectionSettings redundancyDetection = new RedundancyDetectionSettings();
redundancyDetection.isEnabled = false;
redundancyDetection.similarityThreshold = 70;
redundancyDetection.minWords = 12;
redundancyDetection.maxWords = 400000;
caseSettings.redundancyDetection = redundancyDetection;
TopicModelingSettings topicModeling = new TopicModelingSettings();
topicModeling.isEnabled = false;
topicModeling.ignoreNumbers = false;
topicModeling.topicCount = 50;
topicModeling.dynamicallyAdjustTopicCount = false;
caseSettings.topicModeling = topicModeling;
OcrSettings ocr = new OcrSettings();
ocr.isEnabled = true;
ocr.maxImageSize = 12000;
caseSettings.ocr = ocr;

graphClient.compliance().ediscovery().cases("{caseId}").settings()
    .buildRequest()
    .patch(caseSettings);

```