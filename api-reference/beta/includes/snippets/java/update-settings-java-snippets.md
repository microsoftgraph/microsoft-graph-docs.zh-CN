---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1ccb4f6c5f83d5c3f33c61fba9195934a64411b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Settings settings = new Settings();
RedundancyDetectionSettings redundancyDetection = new RedundancyDetectionSettings();
redundancyDetection.isEnabled = false;
redundancyDetection.similarityThreshold = 70;
redundancyDetection.minWords = 12;
redundancyDetection.maxWords = 400000;
settings.redundancyDetection = redundancyDetection;
TopicModelingSettings topicModeling = new TopicModelingSettings();
topicModeling.isEnabled = false;
topicModeling.ignoreNumbers = false;
topicModeling.topicCount = 50;
topicModeling.dynamicallyAdjustTopicCount = false;
settings.topicModeling = topicModeling;
OcrSettings ocr = new OcrSettings();
ocr.isEnabled = true;
ocr.maxImageSize = 12000;
settings.ocr = ocr;

graphClient.compliance().ediscovery().cases("{caseId}").settings()
    .buildRequest()
    .patch(settings);

```