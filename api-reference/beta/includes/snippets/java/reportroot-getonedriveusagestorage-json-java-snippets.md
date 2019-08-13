---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 431b692d533ec68237991fdd4bf6a230857eca51
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360122"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteUsageStorageCollectionPage getOneDriveUsageStorage = graphClient.reports()
    .getOneDriveUsageStorage("D7")
    .buildRequest()
    .get();

```