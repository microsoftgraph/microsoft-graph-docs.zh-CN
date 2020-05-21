---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2044a060b8b4cea9c6a2c4d5132a3c999646b83
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333946"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage owners = graphClient.servicePrincipals("{id}").owners()
    .buildRequest()
    .get();

```