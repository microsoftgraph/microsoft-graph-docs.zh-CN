---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46afaf5a73b91d7bc6a53fb9fbdfbf0ad6028144
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60561869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").resources("517b36a6-9ca2-4e7b-9748-3af25f5cd4fd")
    .buildRequest()
    .get();

```