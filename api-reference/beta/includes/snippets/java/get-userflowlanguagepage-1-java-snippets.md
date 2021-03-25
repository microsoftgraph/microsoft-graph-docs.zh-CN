---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0926ec46aef87eaffba802dbe5cdb6695289c670
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208474"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguagePageCollectionPage defaultPages = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").defaultPages()
    .buildRequest()
    .get();

```