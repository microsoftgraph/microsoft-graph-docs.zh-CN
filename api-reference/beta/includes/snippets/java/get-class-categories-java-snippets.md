---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 354d98e324cbd157f534d543025cf4af39f5a1bb
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991800"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage assignmentCategories = graphClient.education().classes("4797d052-ebf5-4018-a088-e11adc6b2cbb").assignmentCategories()
    .buildRequest()
    .get();

```