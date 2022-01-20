---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4e14384fd11885080edca25c9d707199ee85725
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137744"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryDeltaCollectionPage delta = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignmentCategories()
    .delta()
    .buildRequest()
    .get();

```