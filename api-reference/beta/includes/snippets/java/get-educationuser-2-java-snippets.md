---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efa0c06b46153908c996b9f4af0bdd8ccd7164e7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210556"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("13012")
    .buildRequest()
    .get();

```