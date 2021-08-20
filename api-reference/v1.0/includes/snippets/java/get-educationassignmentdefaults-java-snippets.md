---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e3cb0013a85ad326b164850f7898c46ac2f9c7e67ab3619bd6a61a5deef204d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163510"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignmentDefaults()
    .buildRequest()
    .get();

```