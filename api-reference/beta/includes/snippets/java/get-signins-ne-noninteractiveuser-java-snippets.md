---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9961e25f2defae2418fed5fe86fc1dd2e30de61b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .filter("(signInEventTypes/any(t: t ne 'interactiveUser'))")
    .orderBy("createdDateTime DESC")
    .top(10)
    .get();

```