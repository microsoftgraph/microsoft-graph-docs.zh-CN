---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e483606dfe23a1728710c449b31e84f243e5d45b7963092174278e604d5cbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333560"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}")
    .unsetVerifiedPublisher()
    .buildRequest()
    .post();

```