---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d726a7cab66a7b31005813bdcb8849a3d87b35f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993128"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentCategories("96821157-5efb-4706-8ca2-a90b26c44852")
    .buildRequest()
    .get();

```