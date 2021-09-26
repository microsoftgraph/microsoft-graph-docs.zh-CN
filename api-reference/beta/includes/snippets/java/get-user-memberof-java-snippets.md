---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 069e4f9a1689f728a699d441e9d9fe624291dce309a8be2a1fb677fa8d69892b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.users("{id}").memberOf()
    .buildRequest()
    .get();

```