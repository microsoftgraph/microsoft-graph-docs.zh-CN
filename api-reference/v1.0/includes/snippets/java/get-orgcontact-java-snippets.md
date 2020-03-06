---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95c020a32b102856f43c67228d44ba98c90acd1b
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = graphClient.contacts("{id}")
    .buildRequest()
    .get();

```