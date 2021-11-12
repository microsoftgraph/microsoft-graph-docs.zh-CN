---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f88b2c3cf8b0f84c43d709f16f210dec0b54e05c29b7f6039d85436bd84c778b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903792"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EventCollectionPage events = graphClient.groups("{id}").events()
    .buildRequest()
    .get();

```