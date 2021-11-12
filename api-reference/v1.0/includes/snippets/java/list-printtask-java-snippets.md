---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95251a8a6db8c8da364a25dd214c58c662c99a1327ba6976060a5f75d38efcf0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164285"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskCollectionPage tasks = graphClient.print().taskDefinitions("{taskDefinitionId}").tasks()
    .buildRequest()
    .get();

```