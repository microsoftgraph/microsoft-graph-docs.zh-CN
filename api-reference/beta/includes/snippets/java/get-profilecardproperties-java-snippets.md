---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ecb5302fdef7f04e84f59b2079d13a44e77e080
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968521"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProfileCardPropertyCollectionPage profileCardProperties = graphClient.organization("{organizationId}").settings().profileCardProperties()
    .buildRequest()
    .get();

```