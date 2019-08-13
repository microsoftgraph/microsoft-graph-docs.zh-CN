---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 627979a18ae7436ae343dccd884eb1d6c8d4f0a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308543"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageStorageCollectionPage getMailboxUsageStorage = graphClient.reports()
    .getMailboxUsageStorage("D7")
    .buildRequest()
    .get();

```