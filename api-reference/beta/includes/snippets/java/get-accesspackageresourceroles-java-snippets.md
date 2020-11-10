---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d92894914a0cce27890f2febbe3b903c62b8d09
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageResourceRoleCollectionPage accessPackageResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("15d889df-3eb8-4e9b-bfb4-b1908849aec4").accessPackageResourceRoles()
    .buildRequest()
    .filter("(originSystem+eq+'AadGroup'+and+accessPackageResource/id+eq+'a35bef72-a8aa-4ca3-af30-f6b2ece7208f'),")
    .expand("accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)")
    .get();

```