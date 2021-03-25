---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20f65522daba4fac7167fa107fef777b5bfa5ec8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209833"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.contacts("{id}").manager()
    .buildRequest()
    .get();

```