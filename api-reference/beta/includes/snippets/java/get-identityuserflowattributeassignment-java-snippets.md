---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bd315321e94949b9322875d7e76381de30eb53c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435158"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments()
    .buildRequest()
    .get();

```