---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b67512aa4b3a79499a7f80979c23b0c32cdf0407aad75d66d795dbb11880fd96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .unsubscribeByMail()
    .buildRequest()
    .post();

```