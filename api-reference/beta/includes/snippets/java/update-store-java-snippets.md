---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67e9db518301b32d8cf887fc0376a5ff8b389e7795ea145355bc6a90dde2a812
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Store store = new Store();
store.defaultLanguageTag = "en-US";

graphClient.termStore()
    .buildRequest()
    .patch(store);

```