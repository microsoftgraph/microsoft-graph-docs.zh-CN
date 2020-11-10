---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14e974d5b1450d1109786e5286441a02033e79d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953004"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverride inferenceClassificationOverride = new InferenceClassificationOverride();
inferenceClassificationOverride.classifyAs = InferenceClassificationType.FOCUSED;

graphClient.me().inferenceClassification().overrides("{id}")
    .buildRequest()
    .patch(inferenceClassificationOverride);

```