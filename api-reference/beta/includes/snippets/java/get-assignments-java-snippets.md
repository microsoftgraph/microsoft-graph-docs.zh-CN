---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61886b9ce9821d9b8125a8db498652c5a5fab40f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123637"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments()
    .buildRequest()
    .get();

```