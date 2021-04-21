---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c976c884e7bdb12eaaee314fcebfc90fdfe7d89b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919899"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp").languages()
    .buildRequest()
    .get();

```