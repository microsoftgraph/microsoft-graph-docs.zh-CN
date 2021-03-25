---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d41fba5ad60e474825eaa4a061b340151549797c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210204"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResourceCollectionPage resources = graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").resources()
    .buildRequest()
    .get();

```