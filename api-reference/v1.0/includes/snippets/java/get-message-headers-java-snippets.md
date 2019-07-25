---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beaf797b0dc1d9634447151b74ead9ae0e9f66f2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhAAAW-VPeAAA=")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```