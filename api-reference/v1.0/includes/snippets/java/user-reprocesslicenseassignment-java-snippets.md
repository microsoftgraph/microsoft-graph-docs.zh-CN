---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91dbcaff05b9781f0970189bfa6a94c8a1a2d29f
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953629"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("047dd774-f1c4-40f2-82f0-278de79f9b83")
    .reprocessLicenseAssignment()
    .buildRequest()
    .post();

```