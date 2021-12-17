---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2ba4d4c78adb3df6c76faa7ba905eb6db0656e
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61544905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments()
    .buildRequest()
    .expand("resources")
    .get();

```