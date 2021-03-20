---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bbc5d81882b3b9a9d35c85535004f75d435061c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943483"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.contacts("{id}").manager()
    .buildRequest()
    .get();

```