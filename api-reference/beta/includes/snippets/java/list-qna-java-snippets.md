---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cfa5abccd12e41f554c57c645334ca78c545da5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338398"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

QnaCollectionPage qnas = graphClient.search().qnas()
    .buildRequest()
    .get();

```