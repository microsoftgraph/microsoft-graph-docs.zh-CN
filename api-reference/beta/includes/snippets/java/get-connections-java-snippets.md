---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07ad05af5acd1d8ad247941afb4f4c5613b58d8c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965627"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IExternalConnectionCollectionPage connections = graphClient.external().connections()
    .buildRequest()
    .get();

```