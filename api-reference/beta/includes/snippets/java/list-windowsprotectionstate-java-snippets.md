---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c43fa395e32aab9c679d3a70fb247e80248f45
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsProtectionStateCollectionPage windowsProtectionStates = graphClient.tenantRelationships().managedTenants().windowsProtectionStates()
    .buildRequest()
    .get();

```