---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04b262a678782c65aad0362cccd002cf492a8be
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = new PersonName();
personName.displayName = "Innocenty Popov";
personName.first = "Innocenty";
personName.initials = "IP";
personName.last = "Popov";
personName.languageTag = "en-US";
personName.maiden = null;

graphClient.me().profile().names()
    .buildRequest()
    .post(personName);

```