---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84f80226e27fceac02a788e01bf7ebd340245e9d
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993080"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments()
    .buildRequest()
    .get();

```