---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 689b78ad1c97d65c555ff9357f97c2425a541af7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873261"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityStorageCollectionPage getOffice365GroupsActivityStorage = graphClient.reports()
    .getOffice365GroupsActivityStorage('D7')
    .buildRequest()
    .get();

```