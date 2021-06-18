---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9afa7aaf669d26599fe46f1d8dc3f0227313d57
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryCollectionPage categories = graphClient.education().classes("a17025d0-62a8-4450-9e6e-db31d8c8feb8").assignments("1fdf61ee-c129-4960-9b7c-8df159aa64b0").categories()
    .buildRequest()
    .get();

```