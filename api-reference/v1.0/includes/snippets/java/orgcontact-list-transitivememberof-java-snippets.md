---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b5f68cbbb57bdd7b242672a4d03aae6bb53177ab4e780962273f74964d64fdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.contacts("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```