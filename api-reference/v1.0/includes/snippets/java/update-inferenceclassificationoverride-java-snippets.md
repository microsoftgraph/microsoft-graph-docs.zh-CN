---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75adc22ec21ab0769e0e0a4b578fd988113d0b30f70d8f5028ad0c9fac592ebf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278828"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverride inferenceClassificationOverride = new InferenceClassificationOverride();
inferenceClassificationOverride.classifyAs = InferenceClassificationType.FOCUSED;

graphClient.me().inferenceClassification().overrides("{id}")
    .buildRequest()
    .patch(inferenceClassificationOverride);

```