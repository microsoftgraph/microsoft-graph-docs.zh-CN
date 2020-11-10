---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 945181d61744d639e7e6fda2a6333b6884c23906
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKey trustFrameworkKey = graphClient.trustFramework().keySets("{id}")
    .getActiveKey()
    .buildRequest()
    .get();

```