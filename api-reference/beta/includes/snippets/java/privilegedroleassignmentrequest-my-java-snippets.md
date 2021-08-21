---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40e986960570e6fb686425ea2f7614d061553354090f75920d9c82bab748b04c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219711"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentRequestMyCollectionPage my = graphClient.privilegedRoleAssignmentRequests()
    .my()
    .buildRequest()
    .get();

```