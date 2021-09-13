---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90925ee90d599d61c4476aa1488de197c6111ab386af1a12809fa0784a1037f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguagePageCollectionPage overridesPages = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").overridesPages()
    .buildRequest()
    .get();

```