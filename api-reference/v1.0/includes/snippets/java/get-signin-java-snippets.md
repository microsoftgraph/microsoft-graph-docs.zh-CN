---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d44588cd654e791af4464205d6a0e7691dae814f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473311"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("66ea54eb-6301-4ee5-be62-ff5a759b0100")
    .buildRequest()
    .get();

```