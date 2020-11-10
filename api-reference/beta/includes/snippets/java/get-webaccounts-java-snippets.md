---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3a66007b22bebf186979f9bb08593d0c2309335
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978520"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWebAccountCollectionPage webAccounts = graphClient.me().profile().webAccounts()
    .buildRequest()
    .get();

```