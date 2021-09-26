---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0018ac206d1183cfa414efbb7ecbcd5fbe9c09d346f1ef1536a093869c352ff8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162430"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.users("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```