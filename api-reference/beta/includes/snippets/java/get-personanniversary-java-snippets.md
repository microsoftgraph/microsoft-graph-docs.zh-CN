---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea475527982b6e6572f4eb47ac80a228f55d674280d5daeab61fc4820afc5210
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161669"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .get();

```