---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c62da23d0e4323f4a17ffcf1df698e4691e10505
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878214"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.me().messages("AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='").extensions("Com.Contoso.Referral")
    .buildRequest()
    .get();

```