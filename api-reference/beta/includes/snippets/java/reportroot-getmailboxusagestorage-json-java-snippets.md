---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 787140d9255bcba47c581b0eb9e722194eef521e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageStorageCollectionPage getMailboxUsageStorage = graphClient.reports()
    .getMailboxUsageStorage('D7')
    .buildRequest()
    .get();

```