---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f652ddc56de4bcd7772dfca765eca411d71a648b12e7f48dc2f0aaa83c187ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethod fido2AuthenticationMethod = graphClient.me().authentication().fido2Methods("-2_GRUg2-HYz6_1YG4YRAQ2")
    .buildRequest()
    .get();

```