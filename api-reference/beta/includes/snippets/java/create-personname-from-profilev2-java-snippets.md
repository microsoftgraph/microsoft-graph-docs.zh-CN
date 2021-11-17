---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47895207a4b8a547cacde59ac20db53917d673d91d0fdb9e57d9db7142237f31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279488"
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