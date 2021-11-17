---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea3efe08ba34894ff84630db18c308c704a9417773bad728bb1c517234f5eaab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en")
    .buildRequest()
    .get();

```