---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5104b798b95acfff0735fe4b88363d5c67ba1da
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508702"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c").appliesTo("2441b489-4f12-4882-b039-8f6006bd66da").reference()
    .buildRequest()
    .delete();

```