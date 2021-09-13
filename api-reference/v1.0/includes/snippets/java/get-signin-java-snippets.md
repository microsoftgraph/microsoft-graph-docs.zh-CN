---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c9c43cd0700e97eea16f8a049446d93641ff598ab85f94bff4b645aba1cfd78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105916"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("66ea54eb-6301-4ee5-be62-ff5a759b0100")
    .buildRequest()
    .get();

```