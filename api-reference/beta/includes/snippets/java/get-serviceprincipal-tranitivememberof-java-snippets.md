---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4daa8709bcfe47fd10090f36a1b0722f09cece22666005c25ff3fecd783871a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.servicePrincipals("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```