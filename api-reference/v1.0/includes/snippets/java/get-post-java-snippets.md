---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 841c8e8a221884050e797e810c371888f6b946322aecf2ec33339e603c83b8e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103778"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("{id}").threads("{id}").posts("{id}")
    .buildRequest()
    .get();

```