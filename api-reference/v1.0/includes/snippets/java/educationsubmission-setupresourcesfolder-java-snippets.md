---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd7aaa10e6fb41339eb023a7d2e99fd9e89487ef
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993340"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("d38ffdea-da93-46ac-90ba-d568c6073075").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7")
    .setUpResourcesFolder()
    .buildRequest()
    .post();

```