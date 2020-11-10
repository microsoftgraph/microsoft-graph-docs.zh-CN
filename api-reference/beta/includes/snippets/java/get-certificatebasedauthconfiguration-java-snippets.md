---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac1e18a44a09e8e01b3aee731e00201df76157c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959408"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration("{id}")
    .buildRequest()
    .get();

```