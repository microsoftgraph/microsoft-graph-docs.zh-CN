---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 080ad39defb07bc1ed75cf34f1e56d9400b3dc5dcded3266513a0d869823ed54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationCollectionWithReferencesPage applications = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").applications()
    .buildRequest()
    .get();

```