---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bc1be5dd7501cd0513b62ef82e68789d1de07eaf99316d83bc58695780c9d81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Volunteer";

graphClient.me().calendars()
    .buildRequest()
    .post(calendar);

```