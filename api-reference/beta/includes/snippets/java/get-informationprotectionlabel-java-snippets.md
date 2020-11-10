---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3e57edd2abc7137205db3416b7b9347c679a717
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964682"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InformationProtectionLabel informationProtectionLabel = graphClient.me().informationProtection().policy().labels("{id}")
    .buildRequest()
    .get();

```