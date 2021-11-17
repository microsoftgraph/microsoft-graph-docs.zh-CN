---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbb00b5214fbf69d6785d3e6239808616796c19fc5a608893a1b53edf70a9b97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278944"
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