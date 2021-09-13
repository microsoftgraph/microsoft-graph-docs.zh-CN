---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e4f934854d94e8ae81dc1641c99c7fbda2f419522d92d02649beb61473cc9b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .get();

```