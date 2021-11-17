---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 970fd3c0164f429e828fe6606630a498a10656369fa23040f915bb72f4f74596
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewHistoryDefinitionCollectionPage historyDefinitions = graphClient.identityGovernance().accessReviews().historyDefinitions()
    .buildRequest()
    .get();

```