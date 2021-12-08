---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b50d41fb976b20ba1eedff1dfbf99b3aacbebff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341804"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = graphClient.identityGovernance().entitlementManagement().accessPackages("114d3459-3459-114d-5934-4d1159344d11")
    .buildRequest()
    .get();

```