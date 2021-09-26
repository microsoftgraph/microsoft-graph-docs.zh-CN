---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cf5c558ae1cebcb021f6c086782d6a6a5922959a6f6e5f3515f46d05a432aef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333654"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("66ea54eb-blah-4ee5-be62-ff5a759b0100")
    .buildRequest()
    .get();

```