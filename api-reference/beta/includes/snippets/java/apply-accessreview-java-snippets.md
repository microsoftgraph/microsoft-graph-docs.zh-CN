---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7ae61e6f434c5646ca5b063e9d6b1d7aa36d2b1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951789"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .applyDecisions()
    .buildRequest()
    .post();

```