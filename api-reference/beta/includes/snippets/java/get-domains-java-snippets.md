---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5c9f1ce4bc5cfa83417079d29586f801cc24ac8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963922"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDomainCollectionPage domains = graphClient.domains()
    .buildRequest()
    .get();

```