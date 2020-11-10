---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dce24fa3873acf80090a6616f3269202d65651ac
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965887"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationOutcomeCollectionPage outcomes = graphClient.education().me().assignments("{id}").submissions("{id}").outcomes()
    .buildRequest()
    .get();

```