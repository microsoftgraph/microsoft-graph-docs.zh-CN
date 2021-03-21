---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17f0d6fb6a28e8889c9ef350fae04a3f314340ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977621"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .get();

```