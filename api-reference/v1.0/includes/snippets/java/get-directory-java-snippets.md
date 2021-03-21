---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89871ae93d300e5f07fe8b3265d818f3944ce81c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```