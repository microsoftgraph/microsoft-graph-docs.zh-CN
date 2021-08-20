---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c6ce1bbf7280d4e49a298a1a92ee6b724679289f88571705eabfa3b3b08468a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationCollectionPage applications = graphClient.applications()
    .buildRequest()
    .get();

```