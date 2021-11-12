---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab41568edc05f0b63c286518e2eb60b495ff5a55
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560207"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResource educationSubmissionResource = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").submissions("da443246-384d-673b-32db-bdba9d7f2b51").resources("e19bd829-17ee-4483-88d0-f62b406f367c")
    .buildRequest()
    .get();

```