---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d11810dd8b4d8232f23c761bf12a3869c88eba182bbb04758785c019a005ba64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105146"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("13012")
    .buildRequest()
    .get();

```