---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a01bc731f47dd38e32ffcb314153ab28a70e4caedf4c6d1f91e3b3c214f198d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = graphClient.education().classes("{id}").assignmentDefaults()
    .buildRequest()
    .get();

```