---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83750cdeda67aad4a43e00834055b2d1d60db7ff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("11010").assignments("19002").submissions("33223")
    .buildRequest()
    .get();

```