---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6d8255e788074a07f71386800c9c1589ae5b183
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690099"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("bcd7c908-1c4d-4d48-93ee-ff38349a75c8").federatedIdentityCredentials("d9b7bf1e-429e-4678-8132-9b00c9846cc4")
    .buildRequest()
    .delete();

```