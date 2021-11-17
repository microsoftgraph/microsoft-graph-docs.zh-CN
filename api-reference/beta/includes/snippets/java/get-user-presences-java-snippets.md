---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b33f967025b8ce9d9fb86ff7297c51cc846d2e042c1ca8ba855c9093d5b215f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902400"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.communications().presences("dc74d9bb-6afe-433d-8eaa-e39d80d3a647")
    .buildRequest()
    .get();

```