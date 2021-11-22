---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c091dec69f58481fc1b978623100611726f221428b235c4ff81783657c346457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = new PersonName();
personName.nickname = "Kesha";

graphClient.me().profile().names("{id}")
    .buildRequest()
    .patch(personName);

```