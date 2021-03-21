---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 205e080bc8b6473f9bf257e90f8e25367a9fa441
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955179"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFlowLanguagePageCollectionPage overridesPages = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").overridesPages()
    .buildRequest()
    .get();

```