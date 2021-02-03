---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a47194dc6aad91eda2a34de3abf65be3d666a776
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092332"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationFeatureSummary userRegistrationFeatureSummary = graphClient.reports().authenticationMethods()
    .usersRegisteredByFeature('all','all')
    .buildRequest()
    .get();

```