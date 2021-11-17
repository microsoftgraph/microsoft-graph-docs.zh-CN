---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c994d35e4be1dad97640311a70910dbc990c78d2dc3ba6a00108f6bb3f2d9d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer {Token}"));

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{servicePrincipalId}").synchronization().jobs("{jobId}").schema()
    .buildRequest( requestOptions )
    .get();

```