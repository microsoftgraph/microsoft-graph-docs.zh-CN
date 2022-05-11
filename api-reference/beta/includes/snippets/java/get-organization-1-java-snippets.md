---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81e3dc6a6caae724cd0b19bbcb6fba50a1d876bf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Organization organization = graphClient.organization("84841066-274d-4ec0-a5c1-276be684bdd3")
    .buildRequest()
    .get();

```