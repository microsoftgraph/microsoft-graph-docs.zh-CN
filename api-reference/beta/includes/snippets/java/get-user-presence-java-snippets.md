---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecea66b9c0ecd3b894c097259f95e64998caf85588826bb1a6d5cc05df4da1a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101374"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.users("66825e03-7ef5-42da-9069-724602c31f6b").presence()
    .buildRequest()
    .get();

```