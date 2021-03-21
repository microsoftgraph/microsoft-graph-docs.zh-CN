---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1e8dfc9cd799957e12fd6f54a8b8eaee12fd54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.groups("{id}").memberOf()
    .buildRequest()
    .get();

```