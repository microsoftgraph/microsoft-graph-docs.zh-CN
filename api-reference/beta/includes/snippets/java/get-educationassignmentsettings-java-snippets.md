---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 881f63be6cdd681296124137cb0f84a64e0b7d6fd4333da4c180b3a91fe0617a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220515"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = graphClient.education().classes("{id}").assignmentSettings()
    .buildRequest()
    .get();

```