---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f580daa3c0aecdc8127507ab582bd48e9f96b4438984f635fc39366165c90fc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAnalytics itemAnalytics = graphClient.drives("{drive-id}").items("{item-id}").analytics()
    .buildRequest()
    .get();

```