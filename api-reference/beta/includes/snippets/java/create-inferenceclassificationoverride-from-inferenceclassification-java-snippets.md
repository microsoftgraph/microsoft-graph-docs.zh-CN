---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5bb151f5ca70ac576f5f885a4ef9ed35d8609b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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