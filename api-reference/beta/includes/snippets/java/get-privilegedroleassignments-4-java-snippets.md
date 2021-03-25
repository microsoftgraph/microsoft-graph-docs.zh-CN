---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c2ccc1f7ac49b0d8b0a132a135fd8883a74b0df
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209685"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
    .get();

```