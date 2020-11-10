---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d09adc77a3e009b449ce5222e4487b1d8365c377
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955189"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationRubricCollectionPage rubrics = graphClient.education().me().rubrics()
    .buildRequest()
    .get();

```