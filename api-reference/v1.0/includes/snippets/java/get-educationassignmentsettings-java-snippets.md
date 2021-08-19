---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd560e541cd074b853e3c882d90ba5a98fb5ebf179acb2916ce2672808465db0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218792"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentSettings()
    .buildRequest()
    .get();

```