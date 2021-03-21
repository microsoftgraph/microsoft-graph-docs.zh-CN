---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b25c7f0ef6f20d06fc0bdb6d7964637ce98ed97
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordAuthenticationMethodCollectionPage passwordMethods = graphClient.me().authentication().passwordMethods()
    .buildRequest()
    .get();

```