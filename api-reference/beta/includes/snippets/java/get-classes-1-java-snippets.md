---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a0c3527574233e2362c01e82bd04d28450f1c1d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210525"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionPage classes = graphClient.education().classes()
    .buildRequest()
    .get();

```