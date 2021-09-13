---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a369d10fb10a9c0872a7ce432247f68d8a381bca5068c50fb541916e08b1c18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274221"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = graphClient.policies().permissionGrantPolicies("microsoft-user-default-low")
    .buildRequest()
    .get();

```