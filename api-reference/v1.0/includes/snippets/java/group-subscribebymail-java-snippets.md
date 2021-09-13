---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c29a7c714fb028a915567cc2c18089b45d24ed5f5cc0b05fde69f544cf22f3f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333777"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .subscribeByMail()
    .buildRequest()
    .post();

```