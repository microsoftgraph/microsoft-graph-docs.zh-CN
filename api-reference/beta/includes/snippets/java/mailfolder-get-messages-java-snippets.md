---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05303382fab690f8a6e2b744552537dd6ea28083
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983440"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().mailFolders("AAMkAGVmMDEzM").messages()
    .buildRequest()
    .get();

```