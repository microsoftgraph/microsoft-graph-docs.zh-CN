---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ac40042cc8d6c6a9b35c22a667acd1ae6f05290
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969497"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer {Token}"));

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{servicePrincipalId}").synchronization().jobs("{jobId}").schema()
    .buildRequest( requestOptions )
    .get();

```