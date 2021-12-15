---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c0072c74fc064c5c8b926b0bbe012b88a18e6fb
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525929"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignmentCategories("delta")
    .buildRequest()
    .get();

```