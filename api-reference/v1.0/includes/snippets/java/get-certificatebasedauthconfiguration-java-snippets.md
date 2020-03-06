---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac1e18a44a09e8e01b3aee731e00201df76157c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638709"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration("{id}")
    .buildRequest()
    .get();

```