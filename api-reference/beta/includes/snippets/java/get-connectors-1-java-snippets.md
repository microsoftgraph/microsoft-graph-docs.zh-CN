---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52b82a66e0043cead8e24b90444a29bddebcaaa7857c2121eaab12d1d8a8d514
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220533"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorCollectionPage connectors = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors()
    .buildRequest()
    .get();

```