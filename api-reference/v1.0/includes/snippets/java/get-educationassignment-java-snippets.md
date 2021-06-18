---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71d8ae77bed28b0cd8dc97e3c9363a6bd490f4c4
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992562"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = graphClient.education().classes("5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5").assignments("1fdf61ee-c129-4960-9b7c-8df159aa64b0")
    .buildRequest()
    .get();

```