---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 895af71aabd85d890adbf07fe9b53d098d6e64cb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957882"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConditionalAccessPolicyCollectionPage policies = graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .get();

```