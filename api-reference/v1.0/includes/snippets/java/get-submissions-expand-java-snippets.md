---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73f9d3abc38efd39dc12af1a05979659ce9682d6
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890537"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionCollectionPage submissions = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("efcdf80b-a5de-42ac-8579-e40b0223d48b").submissions()
    .buildRequest()
    .expand("outcomes")
    .get();

```