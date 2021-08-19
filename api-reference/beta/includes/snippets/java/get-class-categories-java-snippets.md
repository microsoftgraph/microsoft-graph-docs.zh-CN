---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ce3a744d6423958fd2ca95214f3c78dd5a52bb77a408f74314154ecf5720150
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage assignmentCategories = graphClient.education().classes("4797d052-ebf5-4018-a088-e11adc6b2cbb").assignmentCategories()
    .buildRequest()
    .get();

```