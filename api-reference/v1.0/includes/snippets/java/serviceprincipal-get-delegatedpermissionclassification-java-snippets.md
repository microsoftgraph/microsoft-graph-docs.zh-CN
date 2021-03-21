---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04560085b56855d6c5aa8c03610872280b38796
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974887"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassificationCollectionPage delegatedPermissionClassifications = graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .get();

```