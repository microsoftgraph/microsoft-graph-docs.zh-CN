---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8750820e44752cf8fc26b2e434f16019bd41837be0054c376338723faedda72b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().contactFolders("{id}")
    .buildRequest()
    .delete();

```