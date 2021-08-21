---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61f8a7368047944e62dc70a5f0e35e57be7be8953a9d6b51ff347c6fb1aba0b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = graphClient.privilegedApproval("{id}")
    .buildRequest()
    .get();

```