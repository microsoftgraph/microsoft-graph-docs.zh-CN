---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05080a5a52f20e8cad4e322bf96a9133f42c814
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("{id}")
    .buildRequest()
    .get();

```