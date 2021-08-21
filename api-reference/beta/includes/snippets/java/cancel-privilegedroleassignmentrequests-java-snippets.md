---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7506773f98f31c6d09171b9b5e2cb5241eabb370a86ca1c963301ba99902695
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .cancel()
    .buildRequest()
    .post();

```