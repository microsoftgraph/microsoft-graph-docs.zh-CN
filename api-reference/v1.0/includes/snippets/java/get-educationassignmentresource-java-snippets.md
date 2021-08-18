---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 461d3b007ab124ad72b1a8ec8c8a737f28470493ba8302ba9de514f3dac7bb3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").resources("8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c")
    .buildRequest()
    .get();

```