---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04d949829033d76595390b7a783fbb6b17864100
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968392"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = graphClient.me().profile().notes("{id}")
    .buildRequest()
    .get();

```