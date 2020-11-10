---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f0bef8886f77f08a2dad4520e8ed8b7bf8d5e7a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956203"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Settings settings = graphClient.customRequest("/me/analytics/settings", Settings.class)
    .buildRequest()
    .get();

```