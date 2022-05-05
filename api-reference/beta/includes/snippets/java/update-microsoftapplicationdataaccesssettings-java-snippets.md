---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de588c9c2caa7f5462673e73da3cd9a3e44d66b4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftApplicationDataAccessSettings microsoftApplicationDataAccessSettings = new MicrosoftApplicationDataAccessSettings();
microsoftApplicationDataAccessSettings.disabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981";

graphClient.organization("{organizationId}").settings().microsoftApplicationDataAccess()
    .buildRequest()
    .patch(microsoftApplicationDataAccessSettings);

```