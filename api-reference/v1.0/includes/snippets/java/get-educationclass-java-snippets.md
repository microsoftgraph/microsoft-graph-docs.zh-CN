---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63953e1072f8b7af87070c317bd6636076734dd6835552b66cff841e393aa952
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("{educationClassId}")
    .buildRequest()
    .get();

```