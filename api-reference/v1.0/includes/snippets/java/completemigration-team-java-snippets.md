---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 309fbe54c0d73aa9e30fe16985e652adc11c8d6b64ca1b33bbda059a8b526f1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5")
    .completeMigration()
    .buildRequest()
    .post();

```