---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50279f5dd0c744009ea67fca48255bba1bd4c57f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975126"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppPlatformUserCounts(period='D7')/content", InputStream.class)
    .buildRequest()
    .get();

```