---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a60b7b738c45d1458f4518e48ce9109a7d7dd7c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "subject-value";
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
message.body = body;
message.inferenceClassification = InferenceClassificationType.OTHER;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```