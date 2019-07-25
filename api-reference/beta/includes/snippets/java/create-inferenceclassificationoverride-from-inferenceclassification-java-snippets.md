---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4ea02f2166fb38e4b3c2f808880b7ee55e85a360
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857487"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverride inferenceClassificationOverride = new InferenceClassificationOverride();
inferenceClassificationOverride.classifyAs = InferenceClassificationType.FOCUSED;
EmailAddress senderEmailAddress = new EmailAddress();
senderEmailAddress.name = "Samantha Booth";
senderEmailAddress.address = "samanthab@adatum.onmicrosoft.com";
inferenceClassificationOverride.senderEmailAddress = senderEmailAddress;

graphClient.me().inferenceClassification().overrides()
    .buildRequest()
    .post(inferenceClassificationOverride);

```