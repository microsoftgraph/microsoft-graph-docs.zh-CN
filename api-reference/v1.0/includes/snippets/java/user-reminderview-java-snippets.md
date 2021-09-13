---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a086a7f33b5fa689c8215b451d06f1d0aa7662fd47580fb0ed5e370586c20be8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserReminderViewCollectionPage reminderView = graphClient.me()
    .reminderView(UserReminderViewParameterSet
        .newBuilder()
        .withStartDateTime("2017-06-05T10:00:00.0000000")
        .withEndDateTime("2017-06-11T11:00:00.0000000")
        .build())
    .buildRequest()
    .get();

```