---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adef783bac886c8deea9723891a76dde334d42f1a37e280fc20a9b201a36bcea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163217"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoles("{id}")
    .selfDeactivate()
    .buildRequest()
    .post();

```