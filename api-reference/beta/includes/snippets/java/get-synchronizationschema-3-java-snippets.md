---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ac40042cc8d6c6a9b35c22a667acd1ae6f05290
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer {Token}"));

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{servicePrincipalId}").synchronization().jobs("{jobId}").schema()
    .buildRequest( requestOptions )
    .get();

```