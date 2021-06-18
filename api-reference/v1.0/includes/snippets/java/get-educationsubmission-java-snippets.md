---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d877f3da5390a6266f39cd360b4aa675e3865fb
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992706"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("11010").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("33223")
    .buildRequest()
    .get();

```