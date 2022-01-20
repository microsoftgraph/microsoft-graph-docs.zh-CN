---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97333424fd5f9f487bd2392008aef67d0b704c56
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationSignInDetailedSummaryCollectionPage applicationSignInDetailedSummary = graphClient.reports().applicationSignInDetailedSummary()
    .buildRequest()
    .get();

```