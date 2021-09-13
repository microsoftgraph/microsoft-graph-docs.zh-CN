---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 972264adc9ba9ec253277cb753fbf75067903d71929086974e49c16377f1d9e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106049"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments()
    .buildRequest()
    .get();

```