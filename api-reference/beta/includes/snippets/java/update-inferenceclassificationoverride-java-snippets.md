---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a14e974d5b1450d1109786e5286441a02033e79d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857463"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverride inferenceClassificationOverride = new InferenceClassificationOverride();
inferenceClassificationOverride.classifyAs = InferenceClassificationType.FOCUSED;

graphClient.me().inferenceClassification().overrides("{id}")
    .buildRequest()
    .patch(inferenceClassificationOverride);

```