---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d60f79968d0a5f39ade15f1a1e3618414ae2afee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111070"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().users("f3a5344e-dbde-48b0-be24-b5b62a243836").assignments()
    .buildRequest()
    .get();

```