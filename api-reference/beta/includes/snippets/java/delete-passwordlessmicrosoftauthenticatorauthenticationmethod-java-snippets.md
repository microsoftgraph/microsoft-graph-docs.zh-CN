---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 221e41a474518c79bb155d2101c17fe11e4a7dc8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968644"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().passwordlessMicrosoftAuthenticatorMethods("R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1")
    .buildRequest()
    .delete();

```