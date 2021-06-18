---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa26de4746892fb193916b9bc3f504b095b9758
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").resources("8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c")
    .buildRequest()
    .get();

```