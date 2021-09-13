---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b2b44bbe94a7fb7cfdfd6d7ce603f0ef1129039edee3f8d91d63f6660f34889
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp").languages()
    .buildRequest()
    .get();

```