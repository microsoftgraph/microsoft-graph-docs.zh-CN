---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82662d2817e916e0c983b0e157d7bff72ccff232
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973288"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverride inferenceClassificationOverride = new InferenceClassificationOverride();
inferenceClassificationOverride.classifyAs = InferenceClassificationType.FOCUSED;

graphClient.me().inferenceClassification().overrides("{id}")
    .buildRequest()
    .patch(inferenceClassificationOverride);

```